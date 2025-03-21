---
title: "Simple Coffee Listing"
description: "This challenge is great for working with Front-end libraries like React, Vue,... You will need to implement a reusable card component with different variables based on the data given."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "JavaScript"
  - "React"
  - "Reusable Components"
  - "Front-end libraries"
lessons:
  - 1-fundamentals/free-hosting-for-web-projects
userStories:
  - Create a coffee listing page that matches the given design.
  - Use React or other Front-end libraries for this challenge.
  - Create a Reusable Card component.
  - The card component should include a picture, name, pricing, rating, and number of votes if exists.
  - The card component should render popular tag, availability status conditionally.
  - Render Coffee list with given data. The data should come from a given API or downloaded JSON file.
  - Users can choose to list all products or just available products.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Simple Coffee Listing | Frontend, React project"
  description: "This project is great for working with Front-end libraries like React, Vue,... You will need to implement a reusable card component with different variables based on the data given."
  keywords:
    - "coffee listing"
    - "react"
    - "front-end libraries"
challengeTexts:
  - Our Collection
  - Introducing our Coffee Collection, a selection of unique coffees from different roast types and origins, expertly roasted in small batches and shipped fresh weekly.
  - All Products
  - Available Now
---

## Learning Goals

By completing this challenge, you will:

- Practice working with Front-end libraries like React, Vue, etc.
- Implement a reusable card component with different variables based on the given data.
- Enhance your HTML, CSS, and JavaScript skills.
- Improve your ability to create interactive web applications.

## Requirements

You should create a web page that includes the following elements:

- Create a coffee listing page that matches the given design.
- Use React or other Front-end libraries for this challenge.
- Create a Reusable Card component.
- The card component should include a picture, name, pricing, rating, and number of votes if exists.
- The card component should render popular tag, availability status conditionally.
- Render Coffee list with given data. The data should come from a given API or downloaded JSON file.
- Users can choose to list all products or just available products.
- Deploy the solution and submit both the Repository URL and Demo URL.

## Technical Details

To fetch the data for the coffee listing, you should make a GET request to the following URL:

```bash
https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/4-frontend-libaries/challenges/group_1/data/simple-coffee-listing-data.json
```

Here's an example of how you can use the `fetch` API in JavaScript to retrieve the JSON data from the provided URL:

```javascript
fetch(
  "https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/4-frontend-libaries/challenges/group_1/data/simple-coffee-listing-data.json"
)
  .then((response) => response.json())
  .then((data) => {
    // Use the data here
  })
  .catch((error) => {
    // Handle any errors here
  });
```

### Instructions for Using a Frontend Library for Coffee Listing Challenge

#### 1. Set Up Your Project:

- Use Create React App to set up a new React project.

#### 2. Create Components:

- Create a reusable Card component to display coffee details.
- Create a CoffeeList component to fetch and render the list of coffee items.

#### 3. Fetch Data:

- Use the fetch API to retrieve coffee data from the provided URL.

#### 4. Render Components:

- Use the CoffeeList component to render the list of coffee items using the Card component.

#### 5. Conditional Rendering:

- Implement conditional rendering for tags and availability status.

#### Example Code

```js
// CoffeeList

import React, { useState, useEffect } from "react";
import Card from "./Card";

function CoffeeList() {
  const [coffeeData, setCoffeeData] = useState([]);

  useEffect(() => {
    // Fetch data and set coffeeData
  }, []);

  return (
    <div className="coffee-list">
      {coffeeData.map((coffee) => (
        <Card key={coffee.id} coffee={coffee} />
      ))}
    </div>
  );
}

export default CoffeeList;
```

## Tech Stack

For this project, you have the flexibility to use HTML, CSS, and JavaScript or a Front-end library like React, Vue, etc. Consider the learning curve and additional setup required when choosing a library.

Good luck with the challenge!
