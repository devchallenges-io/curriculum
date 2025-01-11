---
title: "Weather App"
description: "Weather app has been a popular project to add to many devs' portfolios. In this challenge, you will work with an API to get the current weather of a location."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "JavaScript"
  - "API Integration"
lessons:
  - 1-fundamentals/free-hosting-for-web-projects
userStories:
  - Create a weather app that matches the given design.
  - By default, the user can see the weather of a location (you can choose a location). Alternatively, it could use the current location of the user.
  - Users can see temperature, location, time, wind, high/low temperature, weather status of the selected location.
  - Users can see the temperature of the upcoming 24 hours with 3-hour intervals.
  - Users can see a forecast of the next 5 days with weather status and low/high temperature.
  - Users can see summary weather of large cities such as New York, Copenhagen or Ho Chi Minh City (you can choose 3 cities of your choice).
  - Users can choose to display temperature in Celsius or Fahrenheit.
  - Users can search for a city and see its weather.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Weather App"
  description: "Weather app has been a popular project to add to many devs' portfolios. In this challenge, you will work with an API to get the current weather of a location."
  keywords:
    - "weather app"
    - "API integration"
    - "frontend developer"
challengeTexts:
  - Search city....
  - Other large cities
  - 5-day forecast
---

## Learning Goals

By completing this challenge, you will:

- Build a weather app.
- Work with an API to get the current weather of a location.
- Display temperature, location, time, wind, high/low temperature, and weather status of the selected location.
- Show the temperature of the upcoming 24 hours with 3-hour intervals.
- Provide a forecast of the next 5 days with weather status and low/high temperature.
- Display summary weather of large cities.
- Allow users to choose between Celsius and Fahrenheit.
- Implement city search functionality.
- Deploy the solution and submit Repository URL and Demo URL.

## Requirements

You should create a web page that includes the following elements:

- Create a weather app that matches the given design.
- By default, the user can see the weather of a location (you can choose a location). Alternatively, it could use the current location of the user.
- Users can see temperature, location, time, wind, high/low temperature, and weather status of the selected location.
- Users can see the temperature of the upcoming 24 hours with 3-hour intervals.
- Users can see a forecast of the next 5 days with weather status and low/high temperature.
- Users can see summary weather of large cities such as New York, Copenhagen, or Ho Chi Minh City (you can choose 3 cities of your choice).
- Users can choose to display temperature in Celsius or Fahrenheit.
- Users can search for a city and see its weather.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

To fetch the current weather of a location, you can use an API like [OpenWeatherMap](https://openweathermap.org/). The API provides various endpoints for retrieving weather data.

To display the temperature of the upcoming 24 hours with 3-hour intervals, you can make a GET request to the following endpoint:

```
https://api.openweathermap.org/data/2.5/forecast?q={city}&appid={your_api_key}
```

or

```
https://api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lon}&appid={API key}
```

To display a forecast of the next 5 days, you can make a GET request to the following endpoint:

```
https://api.openweathermap.org/data/2.5/forecast/daily?q={city}&cnt=5&appid={your_api_key}
```

For bonus points, you can consider using a frontend framework like React or Vue.js to build this challenge.

### Instructions for Using a Frontend Library for Weather App Challenge

1. Set Up Your Project:

- Use Create React App to set up a new React project.

2. Create Components:

- Create a WeatherApp component to display the weather app and handle the functionalities.
- Create a CurrentWeather component to render the current weather of a location.
- Create a HourlyForecast component to render the temperature of the upcoming 24 hours.
- Create a DailyForecast component to render the forecast of the next 5 days.
- Create a CityWeather component to render the weather of listed cities.

3. Fetch Data:

- Use the fetch API or a library like Axios to retrieve weather data from the provided API.

4. Render Components:

- Use the resusable components and render to the UI.

5. Temperature Conversion:

- Implement functionality to allow users to choose between Celsius and Fahrenheit.

6. City Search:

- Implement functionality to allow users to search for a city and see its weather.

7. Deployment:

- Deploy your solution and provide the Repository URL and Demo URL for submission.

#### Example Code

```js
// WeatherApp

import React, { useState, useEffect } from "react";

function WeatherApp() {
  const [currentWeather, setCurrentWeather] = useState(null);
  const [hourlyForecast, setHourlyForecast] = useState([]);
  const [dailyForecast, setDailyForecast] = useState([]);
  const [selectedCity, setSelectedCity] = useState("");
  const [searchQuery, setSearchQuery] = useState("");

  useEffect(() => {
    // Fetch current weather and forecast data
  }, [selectedCity]);

  const handleCitySearch = (city) => {
    // Update selected city
  };

  const handleTemperatureUnitChange = (unit) => {
    // Update temperature unit (Celsius or Fahrenheit)
  };

  const handleSearchQueryChange = (event) => {
    // Update search query
  };

  const handleSearch = () => {
    // Trigger city search
  };

  return (
    <div className="weather-app">{/* Render weather app components */}</div>
  );
}

export default WeatherApp;
```

```js
// CurrentWeather

import React from "react";

function CurrentWeather({ weatherData }) {
  return (
    <div className="current-weather">{/* Render current weather data */}</div>
  );
}

export default CurrentWeather;
```

```js
// HourlyForecast

import React from "react";

function HourlyForecast({ forecastData }) {
  return (
    <div className="hourly-forecast">{/* Render hourly forecast data */}</div>
  );
}

export default HourlyForecast;
```

```js
// DailyForecast

import React from "react";

function DailyForecast({ forecastData }) {
  return (
    <div className="daily-forecast">{/* Render daily forecast data */}</div>
  );
}

export default DailyForecast;
```

## Tech Stack

For this project, you have the flexibility to use HTML, CSS, and JavaScript or a Front-end library like React, Vue, etc. Consider the learning curve and additional setup required when choosing a library. If you are not familiar with any Front-end libraries, it is recommended to use Vanilla JavaScript.

Good luck with the challenge!
