---
title: Phase 3
phase: 3
published: true
---

{% assign be_topics = site.data.phase3.topics_be | reverse %}
{% assign fe_topics = site.data.phase3.topics_fe | reverse %}
{% assign all_topics = be_topics | concat: fe_topics %}
{% assign sorted_topics = all_topics | sort: 'date' | reverse | where: "published", "true" %}
{% assign projects = site.data.phase3.projects %}

{% for topic in sorted_topics %}
{{ topic.date | date: "%B %-d" }}
: **{{topic.tag}}**{: .label .{{topic.tag}}-label } {% if topic.page %} [{{ topic.title }}]({% link {{topic.page}} %}){% else %} {{topic.title}} {% endif %}
: {% if topic.post_today %} [Post]({% link posts.md %}){: .label .post-label } {% endif %} {% if projects[topic.project_name] %} [Project]({{ projects[topic.project_name].url }}){:target="_blank"}{:rel="noopener noreferrer"}{: .label .project-label {% if projects[topic.project_name].customize %} #custom-repo-link {% endif %}}{% endif %} {% if topic.code_demo %} [Demo]({{ topic.code_demo }}){:target="_blank"}{:rel="noopener noreferrer"}{: .label .code-demo-label } {% endif %}
{% endfor %}
