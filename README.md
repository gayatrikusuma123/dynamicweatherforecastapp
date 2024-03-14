# Weather Forecast App

# Weather Forecast App Documentation

Table of Contents

1. Introduction

2. Features

3. Dependencies

4. Technologies Used

5. External Libraries

6. Code Structure

7. Usage

8. Detailed Functionality

9. Future Improvements

10. Conclusion

# Introduction

=> The Weather Forecast App is a web application designed to provide users with accurate and up-to-date weather information for any city around the world. 

=> It offers a user-friendly interface for users to input a city name or retrieve weather data based on their current location using the browser's geolocation 
feature.

=> Weather data in a fast and easy-to-use way : We are providing highly recognisable weather products that make working with the weather data a way easier. We work with millions of developers around a clock and believe that these benefits might be suitable for most of applications, up to the complex enterprise systems.

=> A spectrum of ready-to-use weather products

=> Short-term and long-term forecasts, history and observation

=> Any location on the globe

=> Transparent pricing and licensing

Weather apps have become an essential part of our daily lives, offering real-time updates on weather conditions that help us plan our activities and stay prepared for the day ahead. 

Weather impacts our decisions, from choosing the right outfit for the day to planning outdoor events. Learning how to build a weather app not only provides you with valuable coding skills but also empowers you to craft a tool that adds practical value to users' lives. Even if you're new to web development, fear not – we'll break down each stage into easily digestible segments, ensuring that you grasp every concept along the way.

=> What Is a Weather API?

A Weather API (Application Programming Interface) is a web service that provide weather data to developers and businesses. These APIs provide their users with data from official weather sources. Moreover, weather APIs usually provide data to their users with API keys.

There are some features that a good weather API should have. Some of those:

=> Rich Weather Data: A good weather API should provide its users with basic weather information (temperature, humidity, wind speed, precipitation, sunny/cloudy, etc.).

=> Up-to-date Weather Data: This API should provide the most up-to-date weather data possible.

=> Forecasts and Future Data: Another feature that makes a weather API popular is that it provides forecast data. These forecasts can help users plan or make decisions based on the weather.

=> Wide Location Support: A good weather API should provide rich location support to its users. Many users in the global age should also be able to use this API.

=> Stability and Reliability: It is very important for a weather API to have high uptime and the accuracy of the data it provides.

# Features

=> Input Section: Users can input a city name manually or use the "Get Device Location" button to fetch weather data based on their current geographical location.

=> Weather Display Section: Upon successful retrieval of weather data, the application displays various weather parameters including temperature, weather description, location, feels-like temperature, and humidity.

=> Dynamic Weather Icon: The application dynamically changes the weather icon based on the weather condition fetched from the OpenWeatherMap API.

=> Error Handling: The app handles errors gracefully, such as invalid city names or API failures, and provides appropriate error messages to the user.

=> Responsive Design: The application is responsive and adapts well to different screen sizes and devices.

# Dependencies

The Weather Forecast App relies on the following dependencies:

=> OpenWeatherMap API: Used to fetch weather data based on the provided city name or geographical coordinates.

=> Google Fonts API: Imported Google Fonts for styling text content within the application.

# Technologies Used

The Weather Forecast App is built using the following technologies:

To build this app, I used the classic trio of web development - HTML, CSS, and JavaScript. 

The front-end was crafted using HTML for the structure, CSS for the styling, and JavaScript to handle the interactivity and data retrieval.

# HTML5: Used for creating the structure of the web page.

This documentation provides a clear explanation of the structure and functionality of the Weather Forecast App HTML code.

=> Structure Overview

The HTML code consists of the following main sections:

~ Wrapper: This is the main container for the entire Weather Forecast App.

~ Header Section: Displays the title of the application, which is "Weather Forecast App". It also includes a left arrow icon for navigation purposes.

~ Input Section: Allows users to input a city name or retrieve the device's location for weather information.

~ Weather Information Section: Displays weather information such as weather icon, temperature, weather description, location, and additional weather details.

=> Detailed Description

~ Header Section: The header section contains the title of the application, "Weather Forecast App", followed by a left arrow icon, which is implemented using the <i> element with the class bx-left-arrow-alt.

~ Input Section: The input section consists of an input field for entering a city name and a button to get the device's location.

The input field has the following attributes:

~ type="text": Specifies that the input should accept text input.

~ spellcheck="false": Disables spell checking for the input field.

~ placeholder="Enter city name": Displays a placeholder text inside the input field.

~ required: Specifies that the input field is required before submitting the form.

~ The button to get the device's location does not have any specific attributes or classes.

=> Weather Information Section

The weather information section displays various weather-related details, including weather icon, temperature, weather description, location, and additional weather details.

~ Weather Icon: An <img> element is used to display the weather icon. The src attribute is empty, indicating that it will be populated dynamically with the appropriate weather icon.

~ Temperature: Temperature is displayed using a <span> element with the class temp. The temperature value is represented by a <span> element with the class numb, followed by a degree symbol (°), and the unit Celsius (C).

~ Location Display: The location display includes an icon (represented by the <i> element with the class bx-map) and the location coordinates represented by a <span> element.

~ Additional Weather Details: This section includes two columns for displaying additional weather details such as "Feels like" temperature and humidity.

~ Feels Like Temperature: Displays the "feels like" temperature using the <div> element with the class feels. It includes a thermometer icon (represented by the <i> element with the class bxs-thermometer) and the temperature value.

~ Humidity: Displays the humidity using the <div> element with the class humidity. It includes a droplet icon (represented by the <i> element with the class bxs-droplet-half) and the humidity value.

# CSS3: Styled the user interface and applied responsive design principles.

This documentation provides a clear explanation of the CSS styles used in the Weather Forecast App.

Font Import

The `@import` rule is used to import the "Poppins" font from Google Fonts. Different weights of the font (400, 500, 600, 700) are imported, and the display=swap parameter ensures that text using this font is rendered as quickly and as accurately as possible.

Reset Styles

The `*` selector is used to reset default styles by setting margins, padding, and box-sizing to `0`, and setting the base font to "Poppins".

Body Styles

The `body` styles are applied to the entire document, setting it to flex display to center its content both vertically and horizontally. It also sets the background to a linear gradient and text color to white.

Text Selection Styles

The `::selection` pseudo-element is used to style the selected text, setting the text color to a dark color and the background to white.

Wrapper Styles

The `.wrapper` class styles the main container of the app, setting its width, background, border-radius, border, and box-shadow.

Header Styles

The `.wrapper header` styles the header section of the app, setting font size, font weight, color, padding, and border bottom. It also aligns the items horizontally.

Icon Styles

The `header i` styles the icon within the header, setting its font size to 0em to hide it by default, cursor to pointer, and margin-right for spacing.

The `.wrapper.active header i` styles the active state of the header icon when the wrapper has an active class. It adjusts the margin and font size to make the icon visible.

Input Section Styles

The `.wrapper .input-part` styles the input section, setting margin and padding.

The `.wrapper.active .input-part` styles the active state of the input section when the wrapper has an active class, hiding the input section.

Informational Text Styles

The `.input-part .info-txt` styles the informational text within the input section, setting font size, text alignment, padding, border-radius, and margin.

The `.input-part .info-txt.error` styles the error state of the informational text, setting its color to indicate an error.

Humidity Icon Styles

The `.humidity i` styles the humidity icon, setting its font size.

# JavaScript (ES6+): Implemented interactivity and dynamic content updates, including fetching data from the API and handling user input.

This documentation provides a clear explanation of the JavaScript code used in the Weather Forecast App.

DOM Element Selection

The JavaScript code starts by selecting necessary elements from the DOM using document.querySelector() and querySelectorAll() methods. These elements include the wrapper, input section, informational text, input field, location button, weather section, weather icon, and arrow back button.

API Key

An API key (apiKey) is defined for accessing weather data. This key is used to authenticate requests to the OpenWeatherMap API.

Event Listeners

The code sets up event listeners for keyup events in the input field and click events on the location button. These event listeners trigger functions to fetch weather data either by city name or by the device's geolocation.

=> Functions

~ requestApi(city): This function constructs the API URL based on the provided city name and calls the fetchData() function.

~ onSuccess(position): This function is a success callback for the geolocation API. It retrieves the latitude and longitude from the device's position and constructs the API URL accordingly.

~ onError(error): This function is an error callback for the geolocation API. It displays an error message in the informational text element.

~ fetchData(): This function fetches weather data from the OpenWeatherMap API using the constructed API URL. It updates the UI with weather details upon successful retrieval and handles errors gracefully.

~ weatherDetails(info): This function extracts relevant weather information from the API response and updates the UI accordingly. It also dynamically updates the weather icon based on the weather condition ID.

=> Event Listener for Arrow Back Button

An event listener is set up for the arrow back button to hide the weather details section when clicked.

# External Libraries

The Weather Forecast App uses the following external libraries:

=> Google Fonts: Imported the "Poppins" font family from Google Fonts for consistent typography across the application.

# Code Structure

The codebase of the Weather Forecast App is organized into three main components:

=> HTML Structure: Defines the layout and structure of the web page using HTML5 elements such as <header>, <section>, and <div>.

=> CSS Styling: Styles the various elements of the application, including fonts, colors, borders, and layout, to create an appealing user interface.

=> JavaScript Interactivity: Implements dynamic behavior and functionality, including handling user input, fetching data from the API, updating the UI, and error handling.

# Usage

To use the Weather Forecast App, follow these steps:

=> Open the web page in a supported web browser.

=> Enter the name of the city for which you want to retrieve weather information in the input field.

=> Press the "Enter" key or click the "Get Device Location" button to fetch weather data.

=> Upon successful retrieval, the weather information will be displayed in the designated section of the page.

=> If an error occurs during the process, an appropriate error message will be displayed to the user.

# Detailed Functionality

=> Input Handling

The app listens for user input in the city name input field.

When the user presses the "Enter" key, it triggers a function to fetch weather data for the entered city.

If the input field is empty, no action is taken.

=> Geolocation Feature

Clicking the "Get Device Location" button triggers a function to fetch weather data based on the user's current geographical location.

The browser's geolocation API is used to retrieve the latitude and longitude coordinates of the user's device.

Weather data is fetched using these coordinates.

=> Fetching Weather Data

The app constructs the API request URL with the provided city name or geographical coordinates and the OpenWeatherMap API key.

It then sends an HTTP request to the OpenWeatherMap API to fetch weather data.

Upon receiving a response, it parses the JSON data and extracts relevant weather information.

=> Displaying Weather Information

If the API request is successful and weather data is retrieved, the app updates the UI to display the weather information.

This includes updating the weather icon, temperature, weather description, location, feels-like temperature, and humidity.

The weather icon changes dynamically based on the weather condition fetched from the API.

=> Error Handling

If the API request fails or returns an error response, the app displays an appropriate error message to the user.

Error messages include notifying the user of invalid city names or API errors.

Error messages are styled differently to distinguish them from regular informational messages.

# Future Improvements

To enhance the Weather Forecast App, consider implementing the following improvements:

=> Additional Weather Parameters: Display more detailed weather information such as wind speed, atmospheric pressure, and visibility.

=> Unit Conversion: Allow users to toggle between different units for temperature (e.g., Celsius and Fahrenheit) and other weather parameters.

=> Enhanced User Interface: Improve the visual design and layout of the application for a more intuitive and engaging user experience.

=> Geolocation Permission Handling: Provide better handling for geolocation permissions and user consent, especially on mobile devices.

# Conclusion

To sum up, nowadays, there are many platforms where people can get weather data. Among these platforms, weather apps are the fastest and most effective. Today, multiple weather apps serve both on websites and mobile applications. These weather apps usually use weather APIs that provide comprehensive data and provide users with live, historical, and weather forecast data.

The Weather Forecast App provides users with a convenient and user-friendly way to access weather information for any location worldwide. 

By leveraging the OpenWeatherMap API and implementing robust error handling, the app delivers accurate and reliable weather forecasts to users. 

With further enhancements and improvements, it can become an indispensable tool for users to plan their activities based on current weather conditions..
