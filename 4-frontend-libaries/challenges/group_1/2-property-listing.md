---
title: "Property Listing"
description: "This challenge is perfect to improve your Frontend skills from beginner to more advanced. You will need to implement reusable components and filter functionalities."
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
  - Create a property listing page that matches the given design.
  - Use React or other Front-end libraries for this challenge.
  - Create a Reusable Property Card component.
  - The card component should include a thumbnail picture, title, description, capacity, price, and rating.
  - The card component should render superhost tag conditionally.
  - Render Property list with given data. The data should come from a given API or downloaded JSON file.
  - Users can filter properties by location and they can select multiple locations at once.
  - Users can filter properties by superhost.
  - "Users can filter properties by property type: 1 bedroom or 2 bedrooms."
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Property Listing"
  description: "This challenge is perfect to improve your Frontend skills from beginner to more advanced. You will need to implement reusable components and filter functionalities."
  keywords:
    - "property listing"
    - "react"
    - "front-end libraries"
challengeTexts:
  - Peace, nature, dream
  - Find and book a great experience.
---

## Learning Goals

By completing this challenge, you will:

- Improve your Frontend skills from beginner to more advanced.
- Implement reusable components and filter functionalities.
- Enhance your HTML, CSS, and JavaScript skills.
- Gain experience in creating interactive web applications.

## Requirements

You should create a web page that includes the following elements:

- Create a property listing page that matches the given design.
- Use React or other Front-end libraries for this challenge.
- Create a Reusable Property Card component.
- The card component should include a thumbnail picture, title, description, capacity, price, and rating.
- The card component should render superhost tag conditionally.
- Render Property list with given data. The data should come from a given API or downloaded JSON file.
- Users can filter properties by location and they can select multiple locations at once.
- Users can filter properties by superhost.
- Users can filter properties by property type: 1 bedroom or 2 bedrooms.
- Deploy the solution and submit both the Repository URL and Demo URL.

## Technical Details

To fetch the data for the property listing, you should make a GET request to the following URL:

```
https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/4-frontend-libaries/challenges/group_1/data/property-listing-data.json
```

Here's an example of how you can use the `fetch` API in JavaScript to retrieve the JSON data from the provided URL:

```javascript
fetch(
  "https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/4-frontend-libaries/challenges/group_1/data/property-listing-data.json"
)
  .then((response) => response.json())
  .then((data) => {
    // Use the data here
  })
  .catch((error) => {
    // Handle any errors here
  });
```

Good luck with the challenge!

### Instructions for Using a Frontend Library for Property Listing Challenge

1. Set Up Your Project:

- Use Create React App to set up a new React project.

2. Create Components:

- Create a reusable PropertyCard component to display property details.
- Create a PropertyList component to fetch and render the list of properties.

3. Fetch Data:

- Use the fetch API to retrieve property data from the provided URL.

4. Render Components:

- Use the PropertyList component to render the list of properties using the PropertyCard component.

5. Filter Functionality:

- Implement filter functionality for location, superhost, and property type.

#### Example Code

```js
// PropertyList

import React, { useState, useEffect } from "react";
import PropertyCard from "./PropertyCard";

function PropertyList() {
  const [propertyData, setPropertyData] = useState([]);

  useEffect(() => {
    // Fetch data and set propertyData
  }, []);

  return (
    <div className="property-list">
      {propertyData.map((property) => (
        <PropertyCard key={property.id} property={property} />
      ))}
    </div>
  );
}

export default PropertyList;
```

## Tech Stack

For this project, you have the flexibility to use HTML, CSS, and JavaScript or a Front-end library like React, Vue, etc. Consider the learning curve and additional setup required when choosing a library. If you are not familiar with any Front-end libraries, it is recommended to use Vanilla JavaScript.

Good luck with the challenge!
