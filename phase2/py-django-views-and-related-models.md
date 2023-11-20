---
layout: post
title: Django Views and Related Models
topic: Python
category: phase2
parent: Phase 2 Back End
nav_order: 9
published: true
---

## 🗓️ Today's Topics

- Review registration & authentication and troubleshoot issues with login/logout
- Customizing views to handle more complex actions and data
- Review One-to-many (O2M) and Many-to-many (M2M) relationships
- What does your team need to know / resolve / unblock to make progress?

## 🎯 Project: Django Flashcards

Today you and your partner should have the basics of your CRUD app working. You should have a solid start on the CRUD app and be in the middle of writing code for the following:

A logged in user can:

- see a list of all their decks
- see all the cards in one deck
- create a new deck
- add a card to a deck

Editing and deleting cards and decks is _less_ important to the core functionality of this app. If you have the above working, you should move on to allowing a user to:

- select a deck to run through the flashcards in that deck
- see the flashcards in the deck in a random order one by one
- mark a flashcard as correct
- continue to see flashcards in the deck that are marked as incorrect until all flashcards are marked as correct
- change or reset the status of a flashcard 

Ideally there should be a way to reset all the cards in the deck but that is less important than getting the core functionality working.

## ✅ Questions to Guide Your Progress and Check Your Understanding

- Assuming that your user first interacts with your application by looking at a list of their flashcard decks, once they select a deck, what would the user would want to see and do next?
- What would it mean to show one specific deck in the UI? What would the URL for that page be? What data would you need to look up in the view?
- If you want to show one particular flashcard in the browser, how would that work in the urls and the views? What would the URL for that page be? How would you look up the flashcard in the view?
- Do you understand what each line in the view functions you have written for list all decks, show one deck, add a card to a deck are doing? If not, what needs to be clarified for you?
- How do forms work in Django? You should be reasonably comfortable with form objects and how forms are handled in the views.
- Can you create new objects, find objects, and find related objects in the Django shell?
- How does Django know if a user is logged in?

## 🔖 Resources

### Django

- 🍕 [Tips for Using Django's Many-to-Many Field](https://www.revsys.com/tidbits/tips-using-djangos-manytomanyfield/) _This was included in earliers posts too. It's probably the best written explanation of M2M relationships out there, so don't miss it._
- [Django Docs: Related Objects Reference](https://docs.djangoproject.com/en/4.2/ref/models/relations/) _Working with objects that are related to each other via O2M or M2M relationships_
- [Django Docs: Making Queries](https://docs.djangoproject.com/en/4.2/topics/db/queries/) _Queries are what you need to look things up in the database_
- [Creating Interactive Views in Django](https://hackersandslackers.com/creating-django-views/) _Detailed post really breaking down views._
- [Django Slug Tutorial](https://learndjango.com/tutorials/django-slug-tutorial)
- [Django Docs: Built-in Template Tags and Filters](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/)
- [CRC model](http://agilemodeling.com/artifacts/crcModel.htm) _The Class-Responsibility-Collaborator model helps you to reason about how to design your models and relationships._
- [Django Docs: Model Field Reference](https://docs.djangoproject.com/en/4.2/ref/models/fields/) _This is a reference for all the different field types you can use in your models. It's a good place to look if you want to know what options are available for a particular field type._
