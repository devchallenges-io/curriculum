---
title: "Count Down Timer"
description: "Build a count down timer using HTML, CSS, and JavaScript to practice your web development skills. Test your knowledge of HTML and CSS syntax while incorporating JavaScript to create an interactive timer."
isNew: false
sort: 1
nature: "HTML/CSS/JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/javascript-functions

userStories:
  - Create a web page that displays a count down timer.
  - Allow users to set the duration of the timer by selecting the plus or minus buttons, for example, 10 seconds.
  - Toggle the timer when the circle button is clicked.
  - Display the remaining time on the page.
  - Style the page using CSS to make it visually appealing.
  - Use JavaScript to handle the logic of the count down timer and update the page accordingly.
  - Deploy the website to make it accessible for everyone.

seo:
  title: "Count Down Timer | JavaScript project"
  description: "Build a count down timer using HTML, CSS, and JavaScript to practice your web development skills. Test your knowledge of HTML and CSS syntax while incorporating JavaScript to create an interactive timer. This project will help you gain a better understanding of DOM manipulation, event handling, and responsive design. By creating a visually appealing layout and implementing logic for the count down timer, you will enhance your skills in creating interactive web applications. Choose to use vanilla HTML, CSS, and JavaScript or popular frameworks like React or Vue.js to complete this project."
  keywords:
    - "count down timer challenge"
    - "html css javascript project"
challengeTexts:
  - Timer
  - Use the + and - buttons to adjust the time, then press the circle button to start.
---

## Learning Goals

The goals of this project are to help you:

- Understand the basics of HTML, CSS, and JavaScript syntax.
- Learn how to incorporate JavaScript into a web page.
- Practice creating and styling HTML elements.
- Manipulate the DOM using JavaScript.
- Handle events in JavaScript.
- Create a visually appealing layout using CSS.

## Requirements

- Create a web page that displays a countdown timer.
- Allow users to set the duration of the timer by selecting the plus or minus buttons, for example, 10 seconds.
- Toggle the timer when the circle button is clicked.
- Display the remaining time on the page.
- Style the page using CSS to make it visually appealing.
- Use JavaScript to handle the logic of the countdown timer and update the page accordingly.
- Deploy the website to make it accessible for everyone.

## Technical Details

1. **HTML**: Create the structure of the web page.

2. **CSS**: Style the web page to make it visually appealing according to the design.

   - Use the CSS property `transform: scale(0.75);` to style the clock for mobile screens.
   - You can use the provided shadow values or customize it with your own values.

```css
/* Heading Text Shadow */
text-shadow: 2px 2px 0px #35383f;

/* Button Shadow */
box-shadow: 0px 4px 0px 0px #23649b;
```

3. **JavaScript**: Write the logic to handle the countdown timer.

   - Select the buttons and timer display elements using `document.querySelector` or `document.getElementById`.
   - Add event listeners to the buttons to detect clicks using `addEventListener`.
   - Implement functions to increase or decrease the timer duration when the plus or minus buttons are clicked.
   - Implement a function to start/stop the timer when the circle button is clicked.
   - Use `setInterval` to update the remaining time every second.
   - Display the remaining time in the timer display element by setting its `textContent` or `innerHTML` property.
   - Clear the interval when the timer reaches zero.

4. **Deployment**: Make the website accessible for everyone.
   - Deploy the website using a service like GitHub Pages, Netlify, or Vercel.

## Tech Stack

- **HTML**: For creating the structure of the web page.
- **CSS**: For styling the web page and making it responsive.
- **JavaScript**: For adding interactivity and handling the coin flip logic.
