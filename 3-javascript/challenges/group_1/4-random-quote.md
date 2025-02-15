---
title: "Random Quote"
description: "This challenge is an excellent opportunity to gain practical experience in utilizing external APIs within your application. The task involves creating a straightforward application for generating random quotes, which will necessitate the use of an external API."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/javascript-arrays
  - 3-javascript/javascript-async-and-api
userStories:
  - Create a random quote app that matches the provided design.
  - Use HTML to build the basic structure.
  - Include the author name, quote, and tag as per the design specifications.
  - Implement interactivity using vanilla JavaScript.
  - Fetch all quotes using the Fetch API.
  - Display a random quote when users first visit the page.
  - Allow users to see a new random quote by clicking the random button.
  - Enable users to copy the quote to the clipboard.
  - Ensure the page is responsive across different screen sizes.
  - Deploy the solution and submit both the Repository URL and Demo URL.
seo:
  title: "Random Quote | JavaScript project"
  description: "This challenge is an excellent opportunity to gain practical experience in utilizing external APIs within your application. The task involves creating a straightforward application for generating random quotes, which will necessitate the use of an external API. Enhance your JavaScript skills and gain experience in utilizing external APIs by creating a random quote app."
  keywords:
    - "random quote challenge"
    - "html css javascript"
challengeTexts:
  - Random
  - Reset
---

## Learning Goals

By completing this challenge, you will:

- Gain practical experience in utilizing external APIs within your application.
- Learn how to create a random quote app that matches a provided design.
- Improve your HTML, CSS, and JavaScript skills.
- Enhance your ability to create interactive web applications.
- Practice fetching data using the Fetch API.
- Implement interactivity using vanilla JavaScript.

## Requirements

You should create a web page that includes the following elements:

- Create a random quote app that matches the provided design.
- Use HTML to build the basic structure.
- Include the author name, quote, and tag as per the design specifications.
- Implement interactivity using vanilla JavaScript.
- Fetch all quotes using the Fetch API.
- Display a random quote when users first visit the page.
- Allow users to see a new random quote by clicking the random button.
- Enable users to copy the quote to the clipboard.
- Ensure the page is responsive across different screen sizes.
- Deploy the solution and submit both the Repository URL and Demo URL.

## Technical Details

- You can use the provided shadow values or customize it with your own values.

```css
/* Box Shadow */
box-shadow: 447px 304px 151px 0px rgba(0, 0, 0, 0), 286px 195px 138px 0px rgba(0, 0, 0, 0.01),
  161px 110px 117px 0px rgba(0, 0, 0, 0.05), 72px 49px 87px 0px rgba(0, 0, 0, 0.09),
  18px 12px 48px 0px rgba(0, 0, 0, 0.1);
```

- Fetch all the quotes from the API: `https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/3-javascript/challenges/group_1/data/random-quotes.json`. You can use the fetch function to retrieve the data as shown in the example below:

```javascript
fetch(
  "https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/3-javascript/challenges/group_1/data/random-quotes.json"
)
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
2. Create a container element to hold the quote and author information.
3. Use CSS to style the container element with the provided box shadow.
4. Create a button element for generating a random quote.
5. Add event listeners to the button element to fetch and display a random quote from the API.
6. Implement the functionality to copy the quote to the clipboard when clicked.
7. Ensure that the page is responsive by using CSS media queries.
8. Test your application to make sure it works as expected.
9. Deploy your solution to a hosting platform of your choice.
10. Submit the Repository URL and Demo URL for evaluation.

Good luck with the challenge!

### JavaScript Intruction

1. Fetch Quotes from API:

- Use the Fetch API to retrieve quotes from the provided URL.

2. Display Random Quote:

- Write a function to display a random quote from the fetched data.

3. Add Event Listener for Random Button:

- Add an event listener to the button to display a new random quote when clicked.

4. Copy Quote to Clipboard:

- Implement functionality to copy the displayed quote to the clipboard.

```javascript
// Fetch quotes from the API
fetch(
  "https://raw.githubusercontent.com/devchallenges-io/curriculum/refs/heads/main/3-javascript/challenges/group_1/data/random-quotes.json"
)
  .then((response) => response.json())
  .then((data) => {
    const quotes = data;

    function displayRandomQuote() {
      // Function to display a random quote
    }

    displayRandomQuote();

    document
      .getElementById("randomButton")
      .addEventListener("click", displayRandomQuote);

    document.getElementById("copyButton").addEventListener("click", () => {
      // Function to copy quote to clipboard
    });
  })
  .catch((error) => {
    console.error("Error fetching quotes:", error);
  });
```

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
