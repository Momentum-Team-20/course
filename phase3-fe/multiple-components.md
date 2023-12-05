---
layout: topic
title: Multiple Components and Conditional Rendering
topic: JavaScript
category: phase3-fe
parent: Phase 3 Advanced Front End
nav_order: 5
published: true
---

## 🎯 Objectives

- Troubleshooting API requests
- Using multiple components and conditional rendering to create a dynamic UI

## 🏗️ Project: Continuing React Trivia

Be methodical in your approach and don't try to do too much at once. It can help to talk with other developers to break the project down into steps you can take.

Once you have categories showing on the page, make your trivia categories selectable. When a user clicks on a category to select it, you should make a request to get at least 10 questions for that category. The API will let you specify how many questions you want to get back, and it will let you specify the type (e.g., multiple choice).

Once you have a successful request for the questions from the selected category, the next step is to show the questions in the UI. You will need to show one question at at a time with answer choices for that question.

If this is too hard, just show one question to start with so you can see it on the page. Next, show the answer choices for that question (don't worry about the order at first; you can change that later). When you can show one question with its answer choices, then make it possible for the user to see the next question in the list of questions by clicking a button.

**If you read a goal in the project README and don't know how to do it, break it down into smaller goals.**

You may find that you need to do this a few times to break tasks down into a manageable piece. **Keep going until you reach something you can do or at least something you can think about.** This is more than OK: it's a smart way to work, and [it's a valuable skill all software engineers develop](https://www.developerway.com/posts/prison-break-solving-life-as-a-developer).

## 📖 Read | 📺 Watch | 🎧 Listen

Re-visit anything from previous reading/watching/listening sections that you didn't get to, and:

- 📖 [Why React Re-Renders](https://www.joshwcomeau.com/react/why-react-re-renders/)
- 📖 [Lifting State Up](https://react.dev/learn/sharing-state-between-components#lifting-state-up-by-example)
- 📺 [Lifting State Up with Hooks](https://www.youtube.com/watch?v=HF4o9KAZNxw)

### Organizing components and data in React

- 📺 [Using Composition in React to Avoid Prop Drilling](https://youtu.be/3XaXKiXtNjw)
- 📖 [Patterns in JavaScript](https://www.patterns.dev/)
- 📖 [Solving "Prop Drilling" in React](https://blog.logrocket.com/solving-prop-drilling-react-apps/)

## 🔖 References

- [Conditional Rendering in React][react-conditional-render]
- [Managing State in React][react-state]

{% include reference_links.md %}
