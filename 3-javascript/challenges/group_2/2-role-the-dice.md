---
title: "Role The Dice"
description: "Create a web-based dice game with HTML, CSS, and JavaScript to enhance your development abilities. Apply your understanding of HTML and CSS code while adding JavaScript functionality to develop an engaging interactive experience."
isNew: false
sort: 2
nature: "HTML/CSS/JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/javascript-variables-and-data-types
  - 3-javascript/javascript-functions

userStories:
  - Create a web page that allows users to roll a virtual dice.
  - Display the result of the dice roll (a number between 1 and 6) on the page.
  - Add functionality to roll the dice when users select the dice table or press the space key.
  - Style the web page according to the design.
  - Use JavaScript to handle the logic of the dice roll and update the page accordingly.
  - Deploy the website to make it accessible for everyone.

seo:
  title: "Roll The Dice | JavaScript project"
  description: "Create a web-based dice game with HTML, CSS, and JavaScript to enhance your development abilities. Apply your understanding of HTML and CSS code while adding JavaScript functionality to develop an engaging interactive experience."
  keywords:
    - "roll a dice challenge"
    - "html css javascript project"
challengeTexts:
  - Roll the dice
  - Click the screen or press space to roll the dice
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

- Create a web page that allows users to roll a virtual dice.
- Display the result of the dice roll (a number between 1 and 6) on the page.
- Add functionality to roll the dice when users select the dice table or press the space key.
- Style the page using CSS to make it visually appealing.
- Use JavaScript to handle the logic of the dice roll and update the page accordingly.
- Deploy the website to make it accessible for everyone.

## Technical Details

1. **HTML**: Create the structure of the web page.

2. **CSS**: Style the web page to make it visually appealing according to the design.

   - The challenge doesn't require creating the table from scratch; instead, you can style the table using a background image.
     ```css
     /* Table Size */
     .table {
       width: 520px;
       height: 400px;
     }
     ```

````

3. **JavaScript**: Write the logic to handle the dice roll.

   - Select the button and result display elements using `document.querySelector` or `document.getElementById`.
   - Add an event listener to the button to detect clicks using `addEventListener`.
   - Inside the event listener function, generate a random number between 1 and 6 using `Math.random` and `Math.floor`.
     For example:

     ```javascript
     const result = Math.floor(Math.random() * 6) + 1;
     ```

   - Display the result in the result display element by setting its `innerHTML` property to an `<img>` tag with the appropriate image source based on the result.
     For example:

     ```javascript
     const resultDisplay = document.querySelector("#result");
     const imageSource = `dice-${result}.svg`;
     resultDisplay.innerHTML = `<img src="${imageSource}" alt="Dice Result">`;
     ```

4. **Deployment**: Make the website accessible for everyone.
   - Deploy the website using a service like GitHub Pages, Netlify, or Vercel.

## Tech Stack

- **HTML**: For creating the structure of the web page.
- **CSS**: For styling the web page and making it responsive.
- **JavaScript**: For adding interactivity and handling the coin flip logic.
````
