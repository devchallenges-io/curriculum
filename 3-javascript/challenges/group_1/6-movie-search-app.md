---
title: "Movie Search App - OMDb"
description: "The challenge is to create a movie search application using external APIs and advanced JavaScript functionalities. The application will allow users to search for movies and display information about them. To create the application, developers can use APIs such as the OMDB API, which provides movie information such as title, year, plot, and ratings."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/introduction-to-javascript
  - 3-javascript/javascript-dom-and-events
userStories:
  - Create a movie search app that matches the given design.
  - Use HTML to create the basic structure.
  - Add inputs, images, details tags,.. according to the design.
  - Use JavaScript to add interactivity.
  - Users should be able to enter a movie name in the search input.
  - After the search input is filled and users press enter, users should see a movie or `Movie not found` text if there is no movie that matches the searched text.
  - The page should be responsive on different screen sizes.
  - Deploy the solution and submit the Repository URL and Demo URL.
seo:
  title: "Movie Search App - OMDb"
  description: "The challenge is to create a movie search application using external APIs and advanced JavaScript functionalities. The application will allow users to search for movies and display information about them. To create the application, developers can use APIs such as the OMDB API, which provides movie information such as title, year, plot, and ratings. Enhance your JavaScript skills and gain experience in utilizing external APIs by creating a movie search app. This project will help you practice HTML, CSS, and JavaScript, as well as improve your ability to create interactive web applications. By deploying the solution and submitting the Repository URL and Demo URL, you will showcase your work to others."
  keywords:
    - "movie search app"
    - "OMDb API"
challengeTexts:
  - Search movie
  - Movie not found
---

## Learning Goals

The learning goals of this project are to:

- Gain practical experience in utilizing external APIs to fetch movie information
- Practice advanced JavaScript functionalities such as DOM manipulation and event handling
- Improve your HTML and CSS skills in creating a responsive web page
- Enhance your ability to create interactive web applications using vanilla JavaScript

## Requirements

You should create a web page that includes the following elements:

- Create a movie search app that matches the given design.
- Use HTML to create the basic structure.
- Add inputs, images, details tags,.. according to the design.
- Use JavaScript to add interactivity.
- Allow users to enter a movie name in the search input.
- Display a movie or `Movie not found` text if there is no movie that matches the searched text.
- Ensure the page is responsive on different screen sizes.
- Deploy the solution and submit the Repository URL and Demo URL.

## Technical Details

- Fetch movie information from the OMDB API: `https://www.omdbapi.com/`. You can use the fetch function to retrieve the data as shown in the example below:

```javascript
fetch("https://www.omdbapi.com/?apikey=YOUR_API_KEY&s=MOVIE_NAME")
  .then((response) => response.json())
  .then((data) => {
    // Use the data here
  })
  .catch((error) => {
    // Handle the error here
  });
```

## Instructions

To complete this challenge, you can follow these steps:

1. Set up the basic structure of the HTML document.
2. Create the necessary elements according to the given design, such as inputs, images, details tags, etc.
3. Use CSS to style the elements, including the provided box shadow.
4. Add JavaScript code to add interactivity to the application.
5. Allow users to enter a movie name in the search input.
6. Fetch movie information from the OMDB API based on the entered movie name.
7. Display the movie information or `Movie not found` text if there is no movie that matches the searched text.
8. Ensure that the page is responsive by using CSS media queries.
9. Test your application to make sure it works as expected.
10. Deploy your solution to a hosting platform of your choice.
11. Submit the Repository URL and Demo URL for evaluation.

Good luck with the challenge!

### JavaScript Instruction

1. Fetch Movie Information from the OMDB API:

- Use the Fetch API to retrieve movie information from the OMDB API.

2. Display Movie or `Movie not found`:

- Write a function to display the movie information or `Movie not found` text based on the fetched data.

3. Add Event Listener for Search Input:

- Add an event listener to the search input to fetch and display movie information when users press enter.

```javascript
// Fetch movie information from the OMDB API
fetch("https://www.omdbapi.com/?apikey=YOUR_API_KEY&s=MOVIE_NAME")
  .then((response) => response.json())
  .then((data) => {
    const movies = data.Search;

    function displayMovieInfo() {
      // Function to display movie information or `Movie not found` text
    }

    document
      .getElementById("searchInput")
      .addEventListener("keypress", (event) => {
        if (event.key === "Enter") {
          displayMovieInfo();
        }
      });
  })
  .catch((error) => {
    console.error("Error fetching movie information:", error);
  });
```

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
