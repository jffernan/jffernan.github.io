# Project #5 Blog: React Redux Portfolio Project - https://github.com/jffernan/my-react-weather-app
This blog is about my completion of Project #5, React Redux Portfolio Project.  Thankfully, this project is the final project in completing the Full Stack Web Development with React online boot camp program.  The project entailed building a React Redux web app with a few requirements so the project was mostly open-ended.  The project was the opportunity to show what I have learned and show what I know now. 

Briefly, I will explain the advantages of using React:

•	React is built around the concept of components, the building blocks of React apps.  Each component has state (an object with data), and each is in charge of their own rendering - the ‘render()’ method is called whenever the state changes.  Combining multiple components allows to structure code better and to observe a separation of concerns. 

•	React makes code reusable across different parts of a web application.   
 
•	React can be small, and it fits well with jQuery and other frameworks.
 
•	React is also extremely fast, because it uses a virtual DOM, and syncs only the changed parts with the underlying page (accessing the DOM is still the slowest part of a modern web application, which is why the framework gets a performance boost by optimizing it).

I decided to build “My React Weather App”, where you can fetch the current weather by entering a location.  To try my app, clone from GitHub via 'git clone git@github.com:jffernan/my-react-weather-app.git' at your terminal, 'cd' to the new directory, and then run ‘npm install’.  Last, run ‘npm start' to launch your http server.  Note: Weather data fetched from OpenWeatherMap API. When trying my app, you can use my API Key or sign-up for a FREE API key at https://openweathermap.org/.  

To start, I want to recap some general steps that I follow to help in my development process, which I learned through the during the completion of the four other school projects:

1.	Visual what the app will look like.   I sketched out a rough mock of how my app should look like on-screen.  This helped identify what will be my components in the app.

 
2.	Place heavy focus on the user needs and user-friendliness, where the app is easy to understand and use.  For example, give the user multiple options to execute the same action.  In my weather app, I offer the user three ways to fetch current weather.  I also try to imagine how the app should function from the perspective of the user.

3.	KISS aka “keep it simple silly”.  Try to keep the app (and code) as simple as possible.

4.	DRY aka “don’t repeat yourself”.  Don’t repeat code and keep code as short as possible.

5.	With KISS and DRY, code with best practices and current practices in mind like ES6 for Javascript.

6.	Try to observe “separation of concerns” patterns.  For instance, keep HTML code in html file, keep CSS code in css file, keep Javascript code in js file, etc.  For instance, the "business logic" of software is a concern, and the interface through which a user uses this “presentation logic” is another.  The separation of concerns is keeping the code for each of these concerns separate.
Another example is in React, where combining multiple components allow to structure code better and to introduce a separation of concerns.

The following list highlights the key features of My React Weather App:

•	I render a text box form for user to input current location, which highlights when typing occurs, and where user hits ‘enter” on the keyboard to retrieve the weather data.

•	I installed a ‘Fetch Weather’ button where the user points to click on it, as another option besides hitting ‘enter.’

•	I utilized Fetch API to retrieve current weather of a specific location from user input, where weather data is fetched from OpenWeatherMap API.

•	I implemented a map feature that integrates with the GMaps library and renders the map from Google Maps.  The user can select their location from the map to fetch weather, as an alternative to typing the location.

•	I created the capability for the user to save their ‘favorite’ locations in a list along with the abilities to select a location from their ‘favorites’ list to fetch weather and to delete a location.

Thank you for reading my blog!  Visit GitHub to download my app at: https://github.com/jffernan/my-react-weather-app.  Thanks again!
