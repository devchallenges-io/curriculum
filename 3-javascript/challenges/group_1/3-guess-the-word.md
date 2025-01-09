---
title: "Guess The Word Game"
description: "This challenge is great to advance your JavaScript skills. The challenge is to create a small game that tests your data management and DOM manipulation with JavaScript."
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
  - Create a guess the word game that matches the given design.
  - Use HTML to create the basic structure.
  - Use Vanilla JavaScript to add interactivity.
  - Users can see a random scrambled word when the page is first loaded or after users click the random button.
  - Users can enter one letter at a time. After each attempt, the input should automatically focus on the next input if it exists.
  - Users can see the number of wrong answers (tries) and which answers are wrong (mistakes).
  - Users can regenerate a new scrambled word by selecting the random button.
  - Users can reset all inputs, mistakes, and tries by selecting the reset button.
  - When the number of tries or mistakes reaches 6, the game should be reset.
  - When the user completes the game, it should show a '🎉 Success' alert.
  - The page should be responsive on different screen sizes.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Guess The Word Game"
  description: "This challenge is great to advance your JavaScript skills. The challenge is to create a small game that tests your data management and DOM manipulation with JavaScript. Enhance your JavaScript skills and test your data management and DOM manipulation capabilities. This project will help you practice HTML, CSS, and JavaScript, as well as improve your ability to create interactive web applications. By deploying the solution and submitting the Repository URL and Demo URL, you will gain experience in sharing your work with others."
  keywords:
    - "guess the word game challenge"
    - "html css javascript"
challengeTexts:
  - Random
  - Reset
---

## Goals

The goals of this project are to help you:

- Advance your JavaScript skills
- Create a small game that tests your data management and DOM manipulation with JavaScript

## Requirements

You should create a web page that includes the following elements:

- A guess the word game that matches the given design
- HTML structure for the basic elements
- Use Vanilla JavaScript to add interactivity
- Users can see a random scrambled word when the page is first loaded or after users click the random button
- Users can enter one letter at a time. After each attempt, the input should automatically focus on the next input if it exists
- Users can see the number of wrong answers (tries) and which answers are wrong (mistakes)
- Users can regenerate a new scrambled word by selecting the random button
- Users can reset all inputs, mistakes, and tries by selecting the reset button
- When the number of tries or mistakes reaches 6, the game should be reset
- When the user completes the game, it should show a '🎉 Success' alert
- The page should be responsive on different screen sizes
- Deploy the solution and submit Repository URL and Demo URL

## Technical Details

You can use the provided shadow values or customize it with your own values.

```css
/* Button Shadow */
filter: drop-shadow(0px 4px 0px #7b248a);

/* Text box shadow */
box-shadow: 0px 4px 0px 0px #030616;
```

## Implementation Instructions

To implement the guess the word app, follow these steps:

1. Create the HTML structure for the game elements, including the scrambled word display, input fields, buttons, and the success alert.

2. Use Vanilla JavaScript to add interactivity to the game. Implement the following functionalities:

- Generate a random scrambled word when the page is first loaded or when the random button is clicked.
- Allow users to enter one letter at a time. After each attempt, automatically focus on the next input field if it exists.
- Keep track of the number of wrong answers (tries) and display which answers are wrong (mistakes).
- Allow users to regenerate a new scrambled word by clicking the random button.
- Allow users to reset all inputs, mistakes, and tries by clicking the reset button.
- Reset the game when the number of tries or mistakes reaches 6.
- Show a '🎉 Success' alert when the user completes the game.
- Ensure the page is responsive on different screen sizes.

3. Customize the CSS styles for the game elements. You can use the provided shadow values or customize them with your own values.

4. Deploy your solution and submit the Repository URL and Demo URL to complete the challenge.

Remember to test your implementation thoroughly to ensure it meets all the requirements.

Good luck with your implementation!

### JavaScript Example

Here is an example of how you can implement a music player app using vanilla JavaScript.

```javascript
// script.js

const words = ["example", "javascript", "coding", "challenge"];
let currentWord = "";
let tries = 0;
let mistakes = 0;

function scrambleWord(word) {
  // Scramble and return the scrambled word
}

function generateRandomWord() {
  // Generate and display scrambled word
}

function createInputFields(length) {
  // Create number of input fields according to the number of letters
}

function handleInput(event) {
  // Handle input change event
}

function resetGame() {
  // Handle game reset button
}

document
  .getElementById("randomButton")
  .addEventListener("click", generateRandomWord);
document.getElementById("resetButton").addEventListener("click", resetGame);

// Initial load
generateRandomWord();
```

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
