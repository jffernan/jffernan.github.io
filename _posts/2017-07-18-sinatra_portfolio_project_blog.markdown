---
layout: post
title:  "Sinatra Portfolio Project blog"
date:   2017-07-18 18:24:51 +0000
---


Project #2 Blog: Sinatra Portfolio Project

Today, July 13th, 2017, I am starting work on the second portfolio project for Flatiron School Online Software Developer bootcamp program. The project requirement is to build a CRUD app to keep track of something important to a person. These types of apps are generally referred to as CRUD (Create Read Update Delete apps) or simple Content Management Systems.

First off, I am excited to be working on this project compared to the first.  The coursework has picked up since the first project, and has been building upon each lesson on top of each lesson leading to this second project.  Right away, I know what type of app to build.  I have decided to work on a “Restaurant Review” app, which I can easily visually the user interface for and how it will look & work.

Next, I must say I am big on “user friendliness.”  I want to build software that is easy to use and understand for users.  Also, I think the less clicks and moving the mouse around is especially better for the user!  I will definitely try to focus heavily on the user.

I will be starting off with coding the user interface.  As I said above, I will be visualizing how my “Restaurant Review” app will work, how the user will see & use it, and I will focus strongly on the app being very user-friendly and easy to understand!

I like following steps so I grabbed this from the intro video “How to build a CLI Gem” from the 1st project.
1)	Plan your gem, imagine your interface
2)	Start with the project structure – google
3)	Start with the entry point – the file run
4)	Force that to build the user interface
5)	Stub out the interface
6)	Start making things real
7)	Discover objects
8)	Program
9)	
Imagine how the app will run for my user:
1)	Greet user– Welcome to my Restaurant Review app!  Here you can save reviews of your favorite (or not so favorite) restaurants!  Bon Appetit!
2)	Input –Home Page will have links to “signup” and “login” pages. 
3)	CRUD-The user will be able to Create a new restaurant review.  The user will be able to Read an existing review he or another user created. User will be able to update a review, but only those he created.  Last, the user will be able to delete any review he entered, but only those he created.
4)	I plan to have “Restaurant review” contain the name of the restaurant, review content, cuisine, and maybe a review_rating(?).
5)	
After setting up my directory and environment with the necessary folders and setup files, I am ready to begin coding with the MVC architecture in mind.  “MVC” stands for Model-View-Controller.   My app will have three models: User, Review, and Restaurant.  I will start work first on the User MVC, in particular coding out the home page and signup/login processes.

Being efficient (and saving time) is very important.  To start, I have created two templates to help in building out the app.  One is a general file structure, which I will include in the app folder to keep of my progress.  Two, I have a created a CRUD template, which contains generic code for my app controller that would be repetitive (and time-consuming) if I would have to write out this code from scratch.  I’m seeing MVC controllers have the same repetitive code. (For this and future projects, I need to remember to keep track of how long it takes to complete the projects like number of hours.  Doing so with like a stopwatch will help keep me on track and not waste too much time.  My goal is to finish the app in 8-24 hours or under 1 day, which I think is a realistic goal.)

After a couple of hours, I completed the signup/login processes.  I ran “Shotgun” to test them, and it works (and looks) great so far.   In case you are wondering what “Shotgun” is, Shotgun is “a small Ruby gem that makes it easier to develop Rack-based Ruby web applications locally by starting Rack with automatic code reloading. A gem is just a library of code that developers wrote and made free and available to the public. This gem lets us start Rack to have a development server running to test our app. When you start an application with shotgun, all of your application code will be reloaded upon every request. That means if you change anything in your code and save it, when you hit 'Refresh' in your browser, your application will respond with the latest version of your code.”  I’m finding Shotgun is very handy after you make changes in code to be able to see those changes right away!

I also tested the password security, and it works fine!  I am using another gem called Bcrypt to provide password authentication.  I also used the “input type=’password’,” to mask a user’s password with asterisks (i.e. it won’t reveal what the user’s password is as they are typing).  Thankfully, I am not at the point where this project requires styling so all the html views are just plain old text!

Next, I will be tackling the process of coding out the Reviews MVC, which probably will take a little longer than a couple hours since it is more complex…but not too difficult.  Half way done!  So far I have put in about 8 hours.
Alright, I finished my app, today July 18th.  In total, it took about 24 hours or less.  Today and yesterday were all about testing and debugging, fixing errors, and re-testing, etc.  It seemed like I I did “test & re-testing” hundreds of time.  But, that is the process!  Ultimately, I got through it through trial and error…trial and lots of errors.  So, again trial and error.   That’s the learning process through the repetition of doing!  On to the next project.  Thanks for reading my blog!



