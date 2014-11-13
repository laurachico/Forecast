# Forecast


### Overview

The aim of this project is to provide a web application to display the forecast for the day and next 3 days using wunderground Weather API. 

### Setup

To setup the application and run it you will have to unzip the folder and double click on index.html.

### Code

The code that provides the functionality and layout for the application is structured as the following:

* **index.html**: HTML template to display the main and only screen of the application. It will provide the table for the list of weekdays, high and low temperatures displayed in Fahrenheit and weather icon.
* **main.css**: CSS to give the main screen template the desired colors and layout.* **forecast.js**: Namespaced JavaScript and jQuery code to provide all the required functionality to the main screen of the application. Provided with functions: getZipCode to get the zip code that the user has entered and check if it is a valid one and pass it to the getForecast function that makes the Ajax request to the API and displayed the returned forecast information.
### Assumptions
* In order to make the application simple I have just displayed the following information taken from simpleforecast.forecastday array: date.weekday, high.fahrenheit, low.fahrenheit and icon_url.
* To do not wait for the Ajax callback if the user provides a wrong zip code I have created the function getZipCode to check if the zip code is valid or not assuming that a valid zip code has 5 digits.
* If the user enter a valid zip code but the API does not return any information a message will be displayed from the response.error.description returned parsed_json.
****
***Author:*** Laura Chico Tierno

