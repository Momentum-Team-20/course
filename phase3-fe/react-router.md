---
layout: topic
title: Client-side Routing in React
topic: JavaScript
category: phase3-fe
parent: Phase 3 Advanced Front End
nav_order: 9
published: true
---

## 🎯 Objectives

- How are projects coming along? 👀
- Review Login, Register and add Logout
- Using local storage with state to store an auth token
- Client-side routing with [React Router](https://reactrouter.com/en/main)

## 🏗️ Collaborative Project

You should be working from your team task list, referencing your detailed wireframes and user flow outline, and making adjustments to all of these as necessary.

⭐ **Keep in mind that you should _ask_ about any issues you run into with using the API.** The backend code CAN BE CHANGED to accommodate what you need, and it is worth talking about.

Here are some benchmarks for **where you should be by now**:

- At least one component (probably the initial "page" your user is going to see when they arrive at your site) should be built out.
- A login form and request is working, though you may not have fully implemented using the token throughout your app yet.
- You should be able to make GET requests for cards and friends, even if those components are not fully complete yet.

### Goals by the next meeting

- Log in is working, ideally with links or buttons in a header.
- Your user can see a list of cards on the page.
- Your user can click on a card to see the details OR you at least have a detail page for a card built even if your routing is not fully working.
- Your app can make POST requests for creating cards. ⭐ Remember that you can initially hard code values if you don't have the form inputs entirely working yet.
- Your app is deployed to Netlify and working in production (you're checking to see that your deployment is working after every pull request is merged to main, right?).

🚀 Deploy to Netlify **today** if you haven't already.

## 📖 Read | 📺 Watch | 🎧 Listen

- 📖 [React Router Overview: What It Does and Why We Need It](https://reactrouter.com/en/main/start/overview#feature-overview)
- 📺 [Learn React Router v6 in 45 minutes](https://youtu.be/Ul3y1LXxzdU) _This video gets real in-depth fast. Watch through the first 10 minutes or so for the basics._
- 📖 [How to Set Up React Router and Route to Other Components](https://www.freecodecamp.org/news/how-to-use-react-router-version-6/)

### 🗄️ Organizing your files

When you have one component per file (which is how it usually should be), the files can accumulate very quickly. While organizational choices are _very_ subjective, there *are* strategies and organizational patterns that you can follow to structure your files in a React application. You should always follow the practices and conventions established by the team that you work with.

For starters, here are two good takes on how to organize your files.

- [React Folder Structure in 5 Steps](https://www.robinwieruch.de/react-folder-structure/)
- [Delightful React File/Directory Structure](https://www.joshwcomeau.com/react/file-structure/)

## 🔖 References

- [Using React Router][react-router]
- [Organizing your files][react-file-structure]

{% include reference_links.md %}
