---
layout: post
title:  "Project #3 Blog: Rails Portfolio Project"
date:   2017-08-17 00:43:33 -0400
---


Today, August 9th, 2017, I am starting work on the 3rd portfolio project for Flatiron School Online Software Developer bootcamp program. The project requirement is to build a CRUD app to keep track of something important to a person. These types of apps are generally referred to as CRUD (Create Read Update Delete apps) or Content Management Systems.

Now, this project is like the 2nd project, where we also had to build a simple CRUD app using Sinatra.  This project will be more complex than that, as it will involve building the app via Ruby on Rails.   Rails is a framework focused on writing model-driven web applications with a Model-View-Controller(MVC) framework.   There is a helpful guide for getting started with Ruby on Rails.  Learn more at: http://guides.rubyonrails.org/getting_started.html.  I am excited to be working on this project.  The coursework has picked up since the 2nd project, and has been building upon each lesson on top of each lesson leading to this project.

First-off, I am going to blog about some differences between Sinatra and Rails, along with some of the advantages and a few disadvantages of both.  While both are Ruby gems and web frameworks to quickly build web apps (and add other Ruby gems to bundle into the app), Sinatra starts with a blank slate with a one folder and one file, which allows for freedom to build in any way.  This can keep the app folder thin, which uses less memory, and then the app runs quicker. In comparison, Rails is built on the MVC architecture.  By default, upon installation, Rails creates an MVC file structure to start.  Some advantages (differences) that Rails has include:

•	A separate ‘routes.rb’ in the ‘config’ directory. A list of routes and paths can easily be displayed on screen by running ‘rails routes’ or ‘rake routes’ in the terminal.
•	Generators to quickly create MVC files, database table migrations, and related directories.
•	Action View helper methods to save time, like form_builder and link_to.
•	Strong Params” to allow or deny parameters passing into your application code to prevent bad, unwanted data entering the database.
•	A large assortment of validations to test user input with standard error messages for failures.
•	‘Partials’, where you can store reuse of repetitive, duplicate code in partials to keep DRY.  You should never have to duplicate code in Ruby on Rails!
•	Uses the standard, 7 restful routes pattern for URLs, where you know where the user is going.
•	Separate ‘Sessions’ Controller to enable sessions to store user login/logout although this is confusing, compared to Sinatra where the sessions is coded entirely in the Users Controller.  A session consists of a hash of values and a session ID, to identify the hash.  The cookie sent to the client's browser includes the session ID.   The browser sends it to the server on every request from the client.  Rails saves and retrieves values using the ‘session’ method, like Sinatra.
•	Handy Flash helper to display temporary messages, notices, or alerts on the next action like ‘redirect’ and then cleared out.   ‘flash.now’ method is used for ‘flashes’ on rendered pages.
•	Filters: methods that are run "before", "after" or "around" a controller action; example: ‘before_action :require_login’ requires that a user is logged in for an action to be run e.g. show’, ‘edit’, ‘update’, or ‘delete’.
•	Nested Resources: Parent-Child relationship (of has_many with belongs_to) reflected in nested routes.  Provides a child-form that relates to the parent resource. Imagine an application with user profiles. You might represent a person's profile via the RESTful URL of /profiles/1, where 1 is the primary key of the profile. If the person wanted to add pictures to their profile, you could represent that as a nested resource of /profiles/1/pictures, listing all pictures belonging to profile 1. The route /profiles/1/pictures/new allows upload a new picture to profile 1.
•	Scope methods instead of class methods, which keep logic in Model, and try to keep only Actions in Controller.

Now, I have decided to build a “Restaurant Review” app, which I can easily visually the user interface for and how it will look & work.  Next, I must say I am big on “user friendliness.”  I want to build software that is easy to use and understand for users.  Also, I think the less clicks and moving the mouse around is especially better for the user!  I will try to keep it simple for the user aka “KISS,” but still have consistent views and messages to the user. Along those lines, there is the programmer’s principle of DRY, which means “don’t repeat yourself.”  DRY also benefits the user so he/she doesn’t have to repeat the same action or see the same thing such as a duplicate message.  Again, I will try to focus heavily on the user while doing my best to KISS and DRY at the same time!  I want the app to be easy to use, easy to read, and easy to understand for users!

I will be starting off with coding the user “signup/login” interface.  As I said above, I will be visualizing how my “Restaurant Review” app will work, how the user will see & use it, and I will focus strongly on the app being very user-friendly and easy to understand!  I like following steps so I grabbed this from the intro video “How to build a CLI Gem” from the 1st project.

1)	Plan your app, imagine your interface
2)	Start with the project structure – google
3)	Start with the entry point – the file run
4)	Force that to build the user interface
5)	Stub out the interface
6)	Start making things real
7)	Discover objects
8)	Program

Imagine how the app will run for my user:

1)	Greet user– Welcome to my Restaurant Review app!  Here you can save reviews of your favorite (or not so favorite) restaurants!  Bon Appetit!
2)	Input –Home Page will have links to “signup” and “login” pages. 
3)	CRUD-The user will be able to Create a new restaurant review.  The user will be able to Read an existing review he or another user created. User will be able to update a review, but only those he created.  Last, the user will be able to delete any review he entered, but only those he created.
4)	I plan to have “Restaurant review” contain the name of the restaurant, review content, cuisine, and a rating, and date visited.

After running ‘rails new’ to setup the new directory and environment with the necessary folders and setup files, I am ready to begin coding with the MVC architecture in mind.  “MVC” stands for Model-View-Controller.   My app will have three models: User, Review, and Restaurant.  I will start work first on the User MVC, coding out the home page and signup/login processes.

Being efficient (and saving time) is very important.  To start, I have created two templates to help in building out the app.  One is a general file structure to keep of my progress.  Two, I have a created a CRUD template, which contains generic code for my app controller that would be repetitive (and time-consuming) if I would have to write out this code from scratch.  I’m seeing MVC controllers have the same repetitive code. My goal is to finish the app in a couple days or under a week, which I think is a realistic goal.

After a couple days, I completed the signup/login processes.  I tested the password security, and it works fine!  I am using another gem called Bcrypt to provide password authentication.  I also used the “input type=’password’,” to mask a user’s password with asterisks (i.e. it won’t reveal what the user’s password is as they are typing).  Thankfully, I am not at the point where this project requires styling so all the html views are just plain old text with minimal styling!

Next, I will be tackling the process of coding out the Reviews MVC, which probably will take a little longer than a couple hours since it is more complex…but not too difficult.  Half way done!  Next, I coded out the Restaurant and Cuisine MVC. 
Alright, I finished my app today, August 16th!  In total, it took about 5 days or so.  

Today and yesterday were all about testing and debugging, fixing errors, and re-testing, and re-factoring and editing text, etc.  It seemed like I did “test & re-testing” hundreds of time.  But, that is the process!  Ultimately, I got through it through test and re-testing, trial and error…trial and lots of errors.  So, again trial and error.   That’s the learning process through the repetition of doing!  On to the next project.  Thank you for reading my blog!  Please try my app by downloading from GitHub at: https://github.com/jffernan/rails-my-restaurant-review.  Thanks again!
.
