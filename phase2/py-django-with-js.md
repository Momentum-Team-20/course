---
layout: post
title: 🍔 Django with a Side of JavaScript 🍟
topic: Python
category: phase2
parent: Phase 2 Back End
nav_order: 10
published: true
---

## 🗓️ Today's Topics

- Progress report on Flashcards
- Incorporating JavaScript in a Django application

## 🎯 Project: Flashcards

Still working on your project. (っ^з^)♪♬

### Where you should be with Flashcards today

#### These tasks should be pretty much done

A logged in user should be able to...

- see a list of all the decks
- see the cards in a given deck (after it is selected from the list, for instance)
- see the question on a given card with no answer showing
- create a new deck via a web form
- create new cards and associate them with a deck

#### You might still be working on

- A user can run through the deck one card at a time
- A user can click to reveal the answer on a card
- A user can mark a card as answered correctly
- You should be able to record that data somewhere. If decks belong to one user and are not shared, then you could record this on the card itself, but if you have another idea about how to model this, go for it.
- You have some way to show a user how they did at the end of the deck
- Bugs
- Styling: a good solution here to save time would be to use a low-key library like [Water.css](https://watercss.kognise.dev/) or [Picnic.css](https://picnicss.com/)

## 🔖 Resources

### Debugging while you work

Setting a `breakpoint()` can help you figure out what code you need in your views. You can also use the Django shell to test your queries.

- [Django Debug Toolbar docs](https://django-debug-toolbar.readthedocs.io/en/latest/)
- [RealPython Debugging with Pdb](https://realpython.com/python-debugging-pdb/) _The built-in Python debugger (Pdb) lets you set breakpoints in your code._
- [Python debugger commands](https://docs.python.org/3/library/pdb.html#debugger-commands)
- [pdb++](https://github.com/pdbpp/pdbpp) _This is pdb with some additional nice features like syntax highlighting. To use it, you can `pipenv install --dev pdbpp` and it will automatically be used instead of the built-in pdb._

### JavaScript & Django

- [Django and AJAX](https://realpython.com/django-and-ajax-form-submissions/)
- [Fetching Data with AJAX and Django](https://www.brennantymrak.com/articles/fetching-data-with-ajax-and-django) -> This article is really helpful and has really good code examples. Important notes:
  > By including the 'X-Requested-With' header set to 'XMLHttpRequest' [in the AJAX request], the view will be able to check if the request is AJAX or not, and return JSON data instead of HTML.

{% highlight python %}
    # In the view function that handles the fetch (AJAX) request
    # you need to check the headers for the 'X-Requested-With' header
    # if this header is set, then you know the request is a fetch (AJAX) request
    request.headers.get('x-requested-with') == 'XMLHttpRequest'
{% endhighlight %}

- [Working with AJAX in Django](https://testdriven.io/blog/django-ajax-xhr/)
- [MDN: Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) _Remember JS?_ 🥴 _Here's a refresher on using Fetch._
- [Django CSRF with AJAX](https://docs.djangoproject.com/en/4.2/ref/csrf/#ajax)
- [LearnDjango: Static Files and Templates](https://learndjango.com/tutorials/django-static-files)

### ⭐ EXTRA/TMI

- [Django Views the Right Way](https://spookylukey.github.io/django-views-the-right-way/the-pattern.html) _This is a detailed, informative deep dive on function-based views in Django_
- [Understanding the CSRF threat and protection measures](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html)
