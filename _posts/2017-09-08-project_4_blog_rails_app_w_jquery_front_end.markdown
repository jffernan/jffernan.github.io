---
layout: post
title:  "Project #4 Blog: "AJAX is really AJA...""
date:   2017-09-08 16:59:42 -0400
---


This blog is about my completion of Project #4, Rails App with a jQuery Front End.  Thankfully, this project was a short one compared to the last 2 projects.  It took only about 8+ hours to finish this project.  The project requirement was to enhance the web app I built in Project #3 by adding dynamic features through jQuery and an Active Model Serialization JSON backend via Rails API.

Briefly, to recap Project #3, I built a “Restaurant Review” web app, where you can sign-up for & log-in as a user to Create, Read, Update, and Delete (CRUD) reviews of restaurants that you have visited.  You can also view restaurant reviews by other users.  If you would like to try my app, clone from GitHub via 'git clone git@github.com:jffernan/rails-my-restaurant-review' at your terminal, 'cd' to the new directory, then run bundle install, and last, run rails server or 'rails s'.  Last, click on the http link to open my app in your browser.  If you run 'rake db:seed' in the terminal, this will seed the database with fake Users & Reviews.

To start, I will briefly explain what “API“, “jQuery”, “AJAX”, “Active Model Serialization”, “JSON”, and “Backend” all  mean:

1.	Backend – The “backend” refers to the server-side.  Application code and databases both reside on the server.  The opposite of backend is the” frontend”, which is the client (such as the end-user’s browser accessing a web app).

2.	API – API stands for Application Programming Interface.  API is a set of subroutine definitions, protocols, and tools to make building application software easier. In general terms, it is a set of clearly defined methods of communication between various software components.  An API (Application Programming Interface) is a way for one system to interact with another via a well-defined interface. An interface is any endpoint that can be used to take actions and consume data on a given application.
  
In relation to the backend, an application may provide an API for its database system, besides the standard web interface.  The benefit of an API for a database system is the purpose to be used by another system, rather than being viewed by a human, so the data that it transfers is unencumbered by the presentation, preventing the consuming code from having to wade through HTML just to find values.  The theory behind APIs is simply faster data transmissions from the server to the client’s/user’s browser, compared to the longer time it takes for a web page to reload everything like HTML in the browser.  A good API just provides data in the easiest format possible for code to digest.  

3.	JSON - JSON stands for "JavaScript Object Notation.”  JSON is a lightweight, data-interchange, text format and a subset of JavaScript programming language, “a client-side (in the browser) scripting language.”  It is easy for humans to read and write and for machines to parse and generate.  JSON was created as a way to use JavaScript to not only consume data from an API, but also serialize that data for consumption.  Most modern web APIs use JavaScript Object Notation, or JSON, as a standard way of describing and defining data.  JSON is structured a  lot like a Ruby hash, where there are sets of key-value pairs.  Accessing these JSON values are easier compared to traversing the nodes of a tag-based HTML document.  Not only is it more efficient, but it's also a function that's native to the language, rather than needing to build or use a library for parsing XML.  The data size of JSON is also much smaller, which means a more efficient, faster data transfer.

A web API is typically defined “as a set of Hypertext Transfer Protocol (HTTP) request messages, along with a definition of the structure of response messages, which is usually in JSON besides the older Extensible Markup Language (XML) format.”  JSON is a very common data format used for the asynchronous browser/server communication, including as a replacement for XML in AJAX-style systems.

4.	AJAX – AJAX = Asynchronous JAvaScript and XML (where XML stands for EXtensible Markup Language, a structured file format containing information about anything that can be stored, transported or shared.  AJAX is “about loading data in the background and display it on the same webpage, without reloading the whole page.”  AJAX is an “art” of exchanging data with a server, and updating parts of a web page - without reloading the whole page.  Ajax is widely used in client-side programming (e.g. Javascript) to allow for data to be sent & received to & from the database/server.  AJAX is a subset of Javascript, a “client-side (in the browser) scripting language.”

Ajax is short for “Asynchronous JAvascript and XML”, which refers to a set of web development techniques (not an actual programming language) using JavaScript to create asynchronous Web applications.  With Ajax, Web apps can send/retrieve data to be used on a web page to and retrieve (XMLHttpRequest) from a server asynchronously (“in the background”), without interfering with the display and behavior of the existing web page (for example: retrieve data from a database without having to perform a page refresh).  By decoupling the data interchange layer from the presentation layer, Ajax allows for Web pages, and by extension Web applications, to change content dynamically without the need to reload the entire page.
  
Current AJAX practices use the JSON format instead of XML.  The acronym AJAX is misleading; It should be “AJA” for “Asynchronous JAvascript.”  The advantage of using JSON is it is native to JavaScript.  

5.	jQuery - jQuery is a popular lightweight, "write less, do more", JavaScript library/framework that makes it easy to use JavaScript on a website.  The $ is a shortcut for jQuery, and provides an interface to the library.   jQuery is a cross-platform JavaScript library designed to simplify the client-side scripting of HTML. 
 
jQuery's syntax is designed to make it easier to navigate a document, select DOM elements, create animations, handle events, and develop Ajax applications without a browser page refresh.  jQuery also provides capabilities for developers to create plug-ins on top of the JavaScript library.  In summary, jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.  The jQuery library contains some of the following features:

a)	Simple HTML/DOM manipulation/modification. 
b)	CSS manipulation. X
c)	HTML event methods. X
d)	Effects and animations. X
e)	Simple AJA methods. X
f)	Utilities.
g)	Plugins. X

The jQuery library is available as a Ruby gem. After adding ‘gem 'jquery-rails’ gem to Gemfile and run ‘bundle install’, add ‘//= require jquery’ to the JS manifest file.  Rails will now load the jQuery library. As an added benefit, the bundler will update jQuery when new versions are released. 

With regards to AJA, JQuery has many different methods to produce AJA.  jQuery provides several methods for AJA functionality.  With the jQuery AJA methods, you can request text, HTML, XML, or JSON from a remote server using both HTTP Get and HTTP Post - And you can load the external data directly into the selected HTML elements of your web page!  Writing regular AJA code can be a bit tricky, because different browsers have different syntax for AJA implementation. This means that you will have to write extra code to test for different browsers.

These methods can be useful, but it all depends on what task is going to be solved and what the application needs are.  JQuery documentation divides these methods into "High Level" and "Low Level”  interfaces.  The Low Level functions are closer to the browser AJA, more customizable, and more powerful.  The High Level functions have an interface and are simpler, but less powerful because they were created for a use-defined.  In all cases, most of JQuery functions are High Level, except JQuery.AJAX(), which is Low Level.  Using JQuery.AJAX() is the same as $.AJAX().

Writing regular AJA code can be a bit tricky, because different browsers have different syntax for AJA implementation. This means that you will have to write extra code to test for different browsers. However, the jQuery team has taken care of this for us, so that we can write AJA functionality with only one single line of code.

6.	Active Model Serialization (AMS) - Serialization is the process by which we take "executable" code, in our case a Ruby object, and represent it as a string that can be consumed anywhere (remember, the Internet is just strings) and then reconstructed back into usable code.  Serializing a Ruby object retains the state, or current values of all the object's attributes, when turning it into a string, and tells us what one object does look like.  Most of what a modern web API does is gather and serialize objects to be passed to the consuming code as a string over HTTP.  Serialization is “just turning the object into a string, in this case a JSON string.”

ActiveModel::Serializer, or AMS, is a Ruby gem available to use in Rails to serialize resources.  At a basic level, a ‘Model’ model in Rails can have a ModelSerializer serializer, and by default, Rails will use the serializer by calling ‘render json: model’ in the controller, an advantage being an implicit call.  Another important benefit is AMS doesn't require the tedious work of building out JSON strings by hand.  

AMS is modeled after the way Rails handles models and controllers.  Add the gem to # Gemfile #...gem 'active_model_serializers'.  Run ‘bundle install’ to activate the gem.  The gem provides a generator in Rails to generate an ActiveModel::Serializer for a Model (which run in console: ‘rails g serializer model’. 

Now, here is a list of the new features that I added to “My Restaurant Review” web app:

•	I added a 'More' link on Review index page to make AJAX get request to render full review comments from previous truncated view of the specific review.

•	I placed a new link, 'Load Reviews' to render a collection of reviews on each of the User, Review, & Restaurant show pages.

•	I created a new 'Next Review' button on the Review show page to make a JQuery/AJAX get request to render the next review.

•	I enabled the Rails API to submit a AJAX post request to create a New Review, which renders the new instance of the Review object on the same page as the New Review form; located below the inputs form along with a confirmation message that the “review was saved.”

•	I added a new method to the Review prototype.  It is named showRating' to render a confirmation message of the new instance of the Review object’s rating using an ES6 Template Literal.  It will appear below the New Review form after a click on ‘Submit’.

Thank you for reading my blog!  Visit GitHub to download my app at: https://github.com/jffernan/rails-my-restaurant-review.  Thanks again!

