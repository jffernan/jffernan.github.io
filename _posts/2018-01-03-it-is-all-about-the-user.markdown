---
layout: post
title:  "It is all about the user!"
date:   2017-06-22 21:00:02 -0400
---

As a budding full stack software developer, I place a heavy focus on meeting user needs in programming. In short, the user is number one!  Like everyone, I use software, apps, and websites on a daily basis, so I really want to use programs that are "user-friendly."  With that said, I want to build, develop, and work on software programs that offer an excellent, user-friendly UX (User Experience).

What should that experience look like for an end-user?  Here are some good characteristics in user-friendliness.

-The program should be easy to use and convenient. For example, I think the less clicks, the less typing, and the less moving the mouse around, the better for the user.

-The User Interface (UI) should be easy to understand. For example, the text on-screen should be easy to read.  I also think the less technical jargon the better.

-Give the user multiple options to execute the same action.  For example, in submitting form data, the user should be able to hit enter on the keyboard or click a button via mouse (or touch screen like on a mobile app) to save their input.

The full cycle of professional software development - from ideation to completion is: Idea -> Design -> Implement -> Test -> Iterate.  Throughout the development process, and especially at the beginning stage of a new app idea, I try to focus heavily on how the app will work from the user's perspective, such as imagining how the program will look and function for the user.  Visualize what the user will see and how the user will use the program.

Here are some other tips I try to follow in the development process.

-Identify what are the user need(s)?  What user problem(s) exist(s) that the software can try to solve for the user?

-If possible, sketch out a rough mock of how the app should look like on-screen. This can help identify what the components will be in the app, like in using React JavaScript library.

-Develop software that you personally would use yourself!

-KISS aka “keep it simple silly”. Try to keep the app (and code) as simple as possible. Along those lines, in React, best practices are to keep components and any internal state within a component as small as possible. Also, the easiest way to start building is by rendering the data model in the UI, but with no interactivity. Starting with a static version of the app won’t require state yet, because state is reserved only for interactivity, that is, data that changes over time.

-Follow the programmer's DRY principle aka “don’t repeat yourself”. Don’t repeat code and keep code as short as possible.

-Combined with KISS and DRY, code with best practices and current practices in mind, like ES6 for Javascript.

-Try to observe “separation of concerns” (SOC) patterns. For instance, keep HTML code in html file, keep CSS code in css file, keep Javascript code in js file, etc. For instance, the "business logic" of software is a concern, and the interface through which a user uses this “presentation logic” is another. The separation of concerns is keeping the code for each of these concerns separate.

-A similar technique is the single responsibility principle (SRP), that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents in the app, where in React, data can be passed using "props". Props are a way of passing data from parent to child component.

I hope you find this blog helpful!  Thanks for reading!
