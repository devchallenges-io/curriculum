---
title: "Recipe page - HomeChef"
description: "In this challenge, you will work with an API to build a Recipe Page/Application. This will require you to understand the API and make multiple API calls to complete the challenge."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "JavaScript"
  - "React"
  - "Next.js"
  - "API Integration"
lessons:
  - 1-fundamentals/free-hosting-for-web-projects
userStories:
  - Create a recipe page that matches the given design.
  - By default, users can see a list of deserts.
  - "Users can select different categories: Beef, Chicken, Dessert, Lamb, Miscellaneous, Pasta,...."
  - The category list should come from the API.
  - Users can sort recipes by their name or ID.
  - Users can search for recipes by name or instructions or area.
  - Users can select a recipe to redirect to a recipe detail page.
  - On the Recipe detail page, users should see category, area, ingredients and instructions.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Recipe page - HomeChef | Frontend, React project"
  description: "In this challenge, you will work with an API to build a Recipe Page/Application. This will require you to understand the API and make multiple API calls to complete the challenge. This project is great for working with Front-end libraries like React, Vue,..."
  keywords:
    - "recipe page"
    - "API integration"
    - "frontend developer"
challengeTexts:
  - Search recipes and more...
  - Back to categories
---

## Learning Goals

By completing this challenge, you will:

- Build a recipe page/application.
- Work with an API to fetch recipe data.
- Implement sorting and searching functionality.
- Create a recipe detail page to display additional information.

## Requirements

You should create a web page that includes the following elements:

- Create a recipe page that matches the given design.
- By default, users can see a list of deserts.
- Users can select different categories: Beef, Chicken, Dessert, Lamb, Miscellaneous, Pasta,....
- The category list should come from the API.
- Users can sort recipes by their name or ID.
- Users can search for recipes by name or instructions or area.
- Users can select a recipe to redirect to a recipe detail page.
- On the Recipe detail page, users should see category, area, ingredients and instructions.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

To fetch recipe data, you can use the [MealDB API](https://www.themealdb.com/api.php). The API provides various endpoints for retrieving recipe categories and recipe details.

To get recipe categories, you can make a GET request to the following endpoint:

```bash
https://www.themealdb.com/api/json/v1/1/categories.php
```

To get recipe details for a specific recipe ID, you can make a GET request to the following endpoint:

```bash
https://www.themealdb.com/api/json/v1/1/lookup.php?i=52772
```

For bonus points, you can consider using Next.js as the frontend library for this challenge.

### Instructions for Using a Frontend Library for Recipe Page Challenge

#### 1. Set Up Your Project:

- Use Create React App to set up a new React project.

#### 2. Create Components:

- Create a RecipeCategories component to display the recipe categories.
- Create a RecipeDetail component to display the recipe detail page.

#### 3. Fetch Data:

- Use the fetch API or a library like Axios to retrieve recipe data from the provided API.

#### 4. Render Components:

- Use the RecipeCategories component to render the recipe categories.
- Use the RecipeDetail component to render the recipe detail page.

#### 5. Sorting and Searching:

- Implement sorting functionality for recipes by name or ID.
- Implement searching functionality for recipes by name, instructions, or area.

#### 6. Redirect to Recipe Detail Page:

- Allow users to select a recipe and redirect them to the recipe detail page.

#### 7. Display Recipe Details:

- On the Recipe detail page, display the category, area, ingredients, and instructions for the selected recipe.

#### 8. Deployment:

- Deploy your solution and provide the Repository URL and Demo URL for submission.

#### Example Code

```js
// RecipePage

import React, { useState, useEffect } from "react";

function RecipePage() {
  const [recipes, setRecipes] = useState([]);
  const [selectedCategory, setSelectedCategory] = useState("dessert");

  useEffect(() => {
    // Fetch recipe data from the API based on selectedCategory
  }, [selectedCategory]);

  return <div className="recipe-page">{/* Render recipe list */}</div>;
}

export default RecipePage;
```

```js
// RecipeDetail

import React, { useState, useEffect } from "react";

function RecipeDetail({ recipeId }) {
  const [recipe, setRecipe] = useState(null);

  useEffect(() => {
    // Fetch recipe data from the API based on recipeId
  }, [recipeId]);

  return <div className="recipe-detail">{/* Render recipe details */}</div>;
}

export default RecipeDetail;
```

## Tech Stack

For this project, you have the flexibility to use HTML, CSS, and JavaScript or a Front-end library like React, Vue, etc. Consider the learning curve and additional setup required when choosing a library.

Good luck with the challenge!
