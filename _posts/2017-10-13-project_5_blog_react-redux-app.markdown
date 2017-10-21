# Project #5 Blog: React Redux Portfolio Project - https://github.com/jffernan/my-react-weather-app
This blog is about my completion of Project #5, React Redux Portfolio Project.  Thankfully, this project is the final project in completing the Full Stack Web Development with React online boot camp program.  The project entailed building a React-Redux, single-page app (SPA) containing a user interface (UI).  With only a few requirements, the project was mostly open-ended and allowed lots of freedom to choose what to build.  The project was the opportunity to show what I have learned and what I know now. 

Briefly, I will explain the advantages of using React:

•	React is built around the concept of components, the building blocks of React apps.  Each component has state (an object with data), and each is in charge of their own rendering - the ‘render()’ method is called whenever the state changes. 

•	React makes code reusable across different parts of a web application.   
 
•	React can be small, and it fits well with jQuery and other frameworks.
 
•	React is also extremely fast, because it uses a virtual DOM, and syncs only the changed parts with the underlying page (accessing the DOM is still the slowest part of a modern web application, which is why the framework gets a performance boost by optimizing it).

I decided to build “My React Weather App”, where you can fetch the current weather by entering a location.  To try my app, clone from GitHub via 'git clone git@github.com:jffernan/my-react-weather-app.git' at your terminal, 'cd' to the new directory, and then run ‘npm install’.  Last, run ‘npm start' to launch your http server.  Note: Weather data fetched from OpenWeatherMap API. When trying my app, you can use my API Key or sign-up for a FREE API key at https://openweathermap.org/.  

To start, I want to recap some general steps that I follow to help in my development process, which I learned through the during the completion of the four other school projects:

1.	Visual what the app will look like.   I sketched out a rough mock of how my app should look like on-screen.  This helped identify what will be my components in the app.

 
2.	Place heavy focus on the user needs and user-friendliness, where the app is easy to understand and use.  For example, give the user multiple options to execute the same action.  In my weather app, I offer the user two ways to fetch current weather.  I also try to imagine how the app should function from the perspective of the user.

3.	KISS aka “keep it simple silly”.  Try to keep the app (and code) as simple as possible. Along those lines, in React, best practices are to keep components and any internal state within a component as small as possible.  Also, the easiest way to start building is by rendering the data model in the UI, but with no interactivity.  Starting with a static version of the app won’t require state yet, because state is reserved only for interactivity, that is, data that changes over time. 

4.	DRY aka “don’t repeat yourself”.  Don’t repeat code and keep code as short as possible.

5.	With KISS and DRY, code with best practices and current practices in mind like ES6 for Javascript.

6.	Try to observe “separation of concerns” (SOC) patterns.  For instance, keep HTML code in html file, keep CSS code in css file, keep Javascript code in js file, etc.  For instance, the "business logic" of software is a concern, and the interface through which a user uses this “presentation logic” is another.  The separation of concerns is keeping the code for each of these concerns separate.  Another example is in React, where having multiple components allow to structure code better and to introduce a separation of concerns.  A similar technique is the single responsibility principle (SRP), that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents, where data can be passed using props. Props are a way of passing data from parent to child component.

The following list highlights the key features of My React Weather App:

•	I render a text box form for user to input current location, which highlights when typing occurs, and where user hits ‘enter” on the keyboard to retrieve the weather data.

•	I installed a ‘Fetch Weather’ button where the user points to click on it, as another option besides hitting ‘enter.’

•	I utilized Fetch API to retrieve current weather temperature and conditions of a specific location from user input, where weather data is fetched from OpenWeatherMap API.

•	I implemented routes using React-Routing Version 4.0 to provide three navigation links, ‘Home’ page, ‘Map’ page, and ‘About’ page.

•	Within the Map page, I provided a ‘custom link” to Google Maps, which will redirect to Google Maps displaying a map of any location the user has already entered.

Thank you for reading my blog!  Visit GitHub to download my app at: https://github.com/jffernan/my-react-weather-app.  Thanks again!
