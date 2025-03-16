---
title: "Length Converter"
description: "Create a web-based length conversion tool with HTML, CSS, and JavaScript to enhance your web development abilities. Apply your understanding of HTML and CSS syntax and integrate JavaScript functionality to develop a responsive converter."
isNew: false
sort: 1
nature: "HTML/CSS/JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/javascript-recursion
  - 3-javascript/introduction-to-typescript
  - 3-javascript/javascript-async-and-api

userStories:
  - Create a web page that allows users to convert common length units.
  - Provide options for users to select the input unit and output unit.
  - Allow users to enter the value to be converted.
  - Display the converted value on the page.
  - Style the web page according to the design.
  - Use JavaScript to handle the logic of the length converter and update the page accordingly.
  - Deploy the website to make it accessible for everyone.

seo:
  title: "Length Converter | JavaScript project"
  description: "Create a web-based length conversion tool with HTML, CSS, and JavaScript to enhance your web development abilities. Apply your understanding of HTML and CSS syntax and integrate JavaScript functionality to develop a responsive converter."
  keywords:
    - "length converter challenge"
    - "html css javascript project"
challengeTexts:
  - Length Converter
  - Select the input and output units, then enter the value to be converted.
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

- Create a web page that allows users to convert common length units.
- Provide options for users to select the input unit and output unit.
- Allow users to enter the value to be converted and the value being converted.
- Users can click a switch button to swap the positions of the two input fields.
- Style the page using CSS to make it visually appealing.
- Use JavaScript to handle the logic of the length converter and update the page accordingly.
- Deploy the website to make it accessible for everyone.

## Technical Details

1. **HTML**: Create the structure of the web page.

2. **CSS**: Style the web page to make it visually appealing according to the design.

3. **JavaScript**: Write the logic to handle the length converter.

   - Retrieve the data needed for unit conversion using the Fetch API.
   - Select the input and output unit select elements using `document.querySelector` or `document.getElementById`.
   - Add event listeners to the select elements to detect changes using `addEventListener`.
   - Implement a function to handle the conversion logic based on the selected units and input value.
   - Display the converted value in the result display element by setting its `textContent` or `innerHTML` property.

4. **Deployment**: Make the website accessible for everyone.
   - Deploy the website using a service like GitHub Pages, Netlify, or Vercel.

## Tech Stack

- **HTML**: For creating the structure of the web page.
- **CSS**: For styling the web page and making it responsive.
- **JavaScript**: For adding interactivity and handling the length conversion logic.
