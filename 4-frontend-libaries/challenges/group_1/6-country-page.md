---
title: "Country Page - WorldRanks"
description: "Quite often, as a developer, you will have to work with a larger amount of data. In this challenge, you will work with a more complicated set of data of countries and display it in a table."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "JavaScript"
  - "React"
  - "Next.js"
  - "API Integration"
lessons:
  - "1-fundamentals/free-hosting-for-web-projects"
userStories:
  - Create a country ranking page that matches the given design.
  - By default, users can see a list of all countries sorted by population.
  - Users can choose to sort by name alphabetical order or population or area (km²).
  - Users can choose to filter by multiple regions, the regions can be Americas, Antarctic, Africa, Asia, Europe, or Oceania.
  - Users can choose to filter countries that are members of the United Nations.
  - Users can choose to filter countries that are independent.
  - Users can filter/search for countries by their names, regions or subregions.
  - Users can see the total number of countries.
  - Users can select a country and see more details on a country page.
  - On the country page, users can see info like population, area, capital,....
  - On the country page, users can see the neighboring countries.
  - On the country page, when users select a neighboring country, it should redirect to the according country page.
  - "[Optional] The country list is paginated"
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Country Page - WorldRanks"
  description: "Quite often, as a developer, you will have to work with a larger amount of data. In this challenge, you will work with a more complicated set of data of countries and display it in a table."
  keywords:
    - "country page"
    - "API integration"
    - "frontend developer"
challengeTexts:
  - Search by Name, Region, Subregion
  - Member of the United Nations
  - Area (km²)
  - Neighbouring Countries
---

## Learning Goals

By completing this challenge, you will:

- Build a country ranking page/application.
- Work with a more complicated set of data of countries.
- Display the country data in a table.
- Implement sorting and filtering functionality.
- Create a country detail page to display additional information.

## Requirements

You should create a web page that includes the following elements:

- Create a country ranking page that matches the given design.
- By default, users can see a list of all countries sorted by population.
- Users can choose to sort by name alphabetical order or population or area (km²).
- Users can choose to filter by multiple regions, the regions can be Americas, Antarctic, Africa, Asia, Europe, or Oceania.
- Users can choose to filter countries that are members of the United Nations.
- Users can choose to filter countries that are independent.
- Users can filter/search for countries by their names, regions or subregions.
- Users can see the total number of countries.
- Users can select a country and see more details on a country page.
- On the country page, users can see info like population, area, capital,....
- On the country page, users can see the neighboring countries.
- On the country page, when users select a neighboring country, it should redirect to the according country page.
- "[Optional] The country list is paginated"
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

To fetch country data, you can use the [WorldRanks API](https://restcountries.com/). The API provides various endpoints for retrieving country data.

To get all countries sorted by population, you can make a GET request to the following endpoint:

```
https://restcountries.com/v3.1/all?sort=population
```

To get country details for a specific country code, you can make a GET request to the following endpoint:

```
https://restcountries.com/v3.1/alpha/{countryCode}
```

For bonus points, you can consider using a frontend framework like Next.js to build this challenge.

### Instructions for Using a Frontend Library for Country Page Challenge

#### 1. Set Up Your Project:

- Use Create React App to set up a new React project.

#### 2. Create Components:

- Create a CountryRanking component to display the country ranking page.
- Create a CountryDetail component to display the country detail page.

#### 3. Fetch Data:

- Use the fetch API or a library like Axios to retrieve country data from the provided API.

#### 4. Render Components:

- Use the CountryRanking component to render the country ranking page.
- Use the CountryDetail component to render the country detail page.

#### 5. Sorting and Filtering:

- Implement sorting functionality for countries by name, population, or area.
- Implement filtering functionality for countries by regions, United Nations membership, and independence.

#### 6. Redirect to Country Detail Page:

- Allow users to select a country and redirect them to the country detail page.

#### 7. Display Country Details:

- On the country detail page, display information like population, area, capital,....
- On the country detail page, display the neighboring countries.

#### 8. Deployment:

- Deploy your solution and provide the Repository URL and Demo URL for submission.

#### Example Code

```js
// CountryRanking

import React, { useState, useEffect } from "react";

function CountryRanking() {
  const [countries, setCountries] = useState([]);
  const [selectedRegion, setSelectedRegion] = useState("");
  const [selectedSort, setSelectedSort] = useState("population");

  useEffect(() => {
    // Fetch country data from the API based on selectedRegion and selectedSort
  }, [selectedRegion, selectedSort]);

  return <div className="country-ranking">{/* Render country list */}</div>;
}

export default CountryRanking;
```

```js
// CountryDetail

import React, { useState, useEffect } from "react";

function CountryDetail({ countryCode }) {
  const [country, setCountry] = useState(null);

  useEffect(() => {
    // Fetch country data from the API based on countryCode
  }, [countryCode]);

  return <div className="country-detail">{/* Render country details */}</div>;
}

export default CountryDetail;
```

## Tech Stack

For this project, you have the flexibility to use HTML, CSS, and JavaScript or a Front-end library like React, Vue, etc. Consider the learning curve and additional setup required when choosing a library. If you are not familiar with any Front-end libraries, it is recommended to use Vanilla JavaScript.

Alternatively, you can also consider using a frontend framework like Next.js for this project. Next.js is a popular React framework that provides server-side rendering, automatic code splitting, and simplified routing. It offers benefits such as improved performance, better SEO, and a smoother development experience. However, keep in mind that using Next.js may require some additional setup and learning compared to Vanilla JavaScript.

Good luck with the challenge!
