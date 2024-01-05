---
layout: topic
title: Project Checklists
topic: Agile
category: phase4
parent: Phase 4
nav_order: 5
published: true
---

## 🏃‍♀️ Your First Sprint

We're just about ready to dive into the code.

Today you should be finalizing planning and doing research on data, technology, and tools you might need. If you are learning something new to build this project, this weekend is a great time to read documentation and do a short tutorial to get up to speed.

**Daily standup and project check-ins start on Monday!**

📆 You should have calendar invitations for your team's standup and check-in times.

Read the following checklists carefully to make sure you're ready.

### ✅ Checklist for the whole team, before you write code

- MVP is clearly defined and every member of the team knows _exactly_ what you are building.
- You've discussed implementation and know _how_ you are building this product.
- User stories and tasks (**at minimum, for MVP**) have been added to your Trello board _User Stories_ and _Backlog_ lists.
- First tasks are queued, not necessarily assigned, in _Current Sprint_.
- You have [created a team organization on GitHub](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/creating-a-new-organization-from-scratch) and added every team member.
- You have created your project repo or repos on GitHub and made sure everyone is added as a collaborator.
    - A `.gitignore` file is in your repo. You can get one that is specific to your project at [gitignore.io](https://www.toptal.com/developers/gitignore). Even more handy: use this [VS Code extension](https://marketplace.visualstudio.com/items?itemName=codezombiech.gitignore).
    - **Pin GitHub links at the top of your Slack channel**.
- Your team is clear on the Git and GitHub workflow and process for reviewing and merging pull requests.
- Make sure everyone who is working in the same repo is using the same code formatter, linter, and version of Python and/or Node. (You can use [EditorConfig](https://editorconfig.org/) or the [EditorConfig VSCode extension](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) to help with this.)
- **Consider appointing a team lead** who can be responsible for running meetings, leading at check-in, and looking after the Trello board. Even better: rotate this role to share the responsibility and experience.

### ✅ Front-End Checklist

- Have you mapped out a user flow through your app?
- **Wireframes for each interface the user will see**
    - What data will you need on each page or interface? Where is it coming from?
    - What requests will you need to make from the front end?
- Your components are planned out (i.e., you know what components you are building and what they will look like and do when they are done.)
- You have planned the client-side routes you think you will need.
- Are you making forms? Where will you store the data?
- What assets (e.g. images, logos) will you need? Do you have them assembled already? Who is responsible for creating them?
- 🚨 **DON'T COMMIT YOUR SECRET KEYS!** Make sure you are using [environment variables](https://vitejs.dev/guide/env-and-mode.html) for secret keys and sensitive info, like API credentials. Vite is using [dotenv](https://github.com/motdotla/dotenv) to allow you to load environment variables from a `.env` file. 
- Have a general strategy for CSS and design so that you can budget time for it.
    - Are you using a CSS library or framework (e.g. Material UI, Bulma, Tailwind)? What is the general look and feel of your app?
    - Have a plan for UI/UX and design.
- **Make sure more than one person on your team has access to the Netlify dashboard** for your app ([Netlify docs on adding site members](https://docs.netlify.com/accounts-and-billing/team-management/manage-team-members/#manage-site-members)). It would be a good idea to **make a team account for your team and make sure everyone has those log-in credentials**.
    - Deploy early.
    - Keep an eye on your production app to ensure that your app continues to work in production.
    - Every time you merge a pull request and the main branch changes, it will trigger a new deploy, so you should check and test your app to confirm that your newest code is working in production after every merge.

### ✅ Back-end Checklist

- **Models!** How will you represent the _nouns_ your project needs?
    - What fields belong on those models? Use the [Django Model Field Reference](https://docs.djangoproject.com/en/4.0/ref/models/fields/).
    - What relationships exist between the models? (one-to-many, many-to-many?)
        - Consider using [the CRC model](http://agilemodeling.com/artifacts/crcModel.htm) to help guide your discussions.
        - You should create an ER (entity relationship) diagram for your models to map relationships. This may change as you work, but you should have thought through and documented your plan to start with.
- What data will the front end rely on the back end for?
- What endpoints will you need to deliver that data?
    - Are you returning HTML? What templates does the front end need, and who will make those?
    - Are you returning JSON? How will you structure your data?
- 🚨 Make sure you are using `django-environ` and a `.env` file. This will be especially important for secret keys and sensitive info, like AWS credentials. **DON'T COMMIT YOUR SECRET KEYS!**
- Make sure you are using Postgres and not SQLite.
- Deploy early.
    - Make sure more than one person on your team has access to the deployment dashboard on whatever service you are using.
    - Make sure that you keep an eye on your production app! Every time you merge a pull request and the main branch changes, it will trigger a new deploy, so you should check and test your app to confirm that your newest code is working in production.
- Put documentation in place early and make sure your front end has access to it.
