---
layout: post
title:  "CLI Data Gem Project blog"
date:   2017-07-05 21:24:04 +0000
---


Project #1: CLI Data Gem Project blog

Today, (June 24th), I am starting for the first project, CLI Data Gem Project, to build a CLI ruby app that scrapes data for a web page.  Reading the instructions, it seems simple enough, but deciding on what to build is the hard part to start, for me at least.  There are 3 examples to look at, and yes, all 3 are very simple (Daily Deals, Now Playing-Movies, 50 Best Restaurants.

What to build?  Two choices keep coming up.  One is a weather CLI app, where you type in your zip code, and get the current weather condition and temperature.  Again, it seems very simple.  My final choice is to build a favorite comic book superhero app, that describes info about a popular Marvel superhero that the user wants to learn about.  I am leaning towards this just because I use to collect comic books as a kid and love all the recent Marvel films!

I like following steps so I grabbed this from the intro video “How to build a CLI Gem.”

1.	Plan your gem, imagine your interface
2.	Start with the project structure – google
3.	Start with the entry point – the file run
4.	Force that to build the CLI interface
5.	Stub out the interface
6.	Start making things real
7.	Discover objects
8.	Program

Interesting, the only step involves programming is the last step.  I like the suggestion to imagine how the program will work from the user’s perspective so I will start there.  I will follow the basic flow of a CLI app that was discussed in a previous lesson: 1. Greet the user, 2.	Ask the user for input, 3. Capture and store that input, and 4. Do something with that input.
Imagine how the app will run for my user:

Greet – Welcome to my CLI app on learning about your favorite Marvel comic book superhero!
Input – Here is a list of the most popular Marvel characters. Please choose one.
Store the input - Let’s say the user chooses “Spiderman” from the list
Do the input – The app should grab and return info about “Spiderman” in the form of a short bio. 

To describe the process, I first began writing the CLI text the user would see displayed and coded it.  Easy!  I then started on the coding of the data scraper.  The challenging part at first was finding a good website with a list of superheroes to scrape.  After several Google searches, I found a “top-12” list on thoughtco.com.  Now, I considered using Marvel’s website and Wikipedia for a list of heroes, but as we all know, Marvel has a billion characters so that would be next to impossible to scrape that large a list.

Next, I coded out the scraper where the first data scrape retrieves the initial list of heroes for the user to choose from.  Then, the second data scrap retrieves a bio on the hero the user has selected.  I coded out options for the user to re-show the list of heroes again to select another hero or type “exit” to quit the program.

Overall, as I thought from the beginning, this was a simple, easy program to build.  I finally completed this project on July 3rd. It took about a week to finish because I flip-flopped several times on building a weather CLI app or a superhero CLI.  I began with the weather CLI app and easily coded the CLI interface to ask the user for their zip code.  However, I could not find any weather websites to successfully scrape the current weather condition and temperature from the user’s input of their zip code.  Also, a weather app would not meet the initial project requirement to show the user a list of available data to choose from. At the most, this project should have only taken a day or two to complete, but…

What was most time-consuming for me was successfully building (setting up) my app as a gem, which wasn’t covered thoroughly in previous lessons.  Learn.com provided a couple other websites on Ruby Gems documentation which helped.  Ultimately, I got through it through trial and error…trial and lots of errors!  Also, this was the first time using git and GitHub on my own and had to learn on my own how to go back to a previous version after several Ruby Gem errors.  It wasn’t very clear on the GitHub documentation how to do so.  So, again trial and error.   That’s the learning process!  On to the next project.  Thanks for reading my blog!







