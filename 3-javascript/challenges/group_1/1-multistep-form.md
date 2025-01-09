---
title: "Multi-step Register Form"
description: "This challenge offers a great opportunity to enhance your JavaScript skills by creating a 3-step registration form with distinct sections, allowing you to test and improve your JavaScript proficiency."
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
  - Create a multi-step registration page that matches the given design.
  - Use HTML to create the basic structure.
  - Add form, inputs, buttons, stepper,... according to the design.
  - "Add validations to the inputs: name and email input should be required and email input should only accept email format."
  - Use Vanilla JavaScript to add interactivity.
  - Users should not be able to continue to the next step if inputs are empty or the topic is not selected.
  - Users can continue to the next step if inputs are filled or topic is selected.
  - Users should know which step they are at.
  - When users click confirm, they should see an alert with '✅ Success' message.
  - The page should be responsive on different screen sizes.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Multi-step Register Form Challenge"
  description: "Create a 3-step registration form using HTML, CSS, and JavaScript. Enhance your JavaScript skills by creating a web page that allows users to register with distinct sections and test their JavaScript proficiency. This project will help you practice HTML, CSS, and JavaScript, as well as improve your ability to create interactive web forms. By deploying the solution and submitting the Repository URL and Demo URL, you will gain experience in sharing your work with others."
  keywords:
    - "multi-step register form challenge"
    - "html css javascript"
challengeTexts:
  - Register
  - Name
  - Enter your name
  - Email
  - Example@gmail.com
  - Continue
  - Step 1 of 3
  - Step 2 of 3
  - Step 3 of 3
  - Which topics you are interested in?
  - Software Development
  - User Experience
  - Graphic Design
  - "Name: Emily Johnson"
  - "Email: emily@emilyjohnsonstl.com"
  - "Topics:"
---

## Goals

The goals of this project are to help you:

- Enhance your JavaScript skills
- Create a 3-step registration form with distinct sections
- Test and improve your JavaScript proficiency

## Requirements

You should create a web page that includes the following elements:

- A multi-step registration page that matches the given design
- HTML structure for the form, inputs, buttons, stepper, etc.
- Validations for the inputs: name and email input should be required and email input should only accept email format
- Use Vanilla JavaScript to add interactivity
- Users should not be able to continue to the next step if inputs are empty or the topic is not selected
- Users can continue to the next step if inputs are filled or topic is selected
- Users should know which step they are at
- When users click confirm, they should see an alert with '✅ Success' message
- The page should be responsive on different screen sizes

## Technical Details

You can use the provided shadow and gradient values or customize it with your own values.

```css
/* Button Gradient */
background: linear-gradient(180deg, #845eee 0%, #652cd1 100%);

/* Border Gradient */
background: linear-gradient(
  120deg,
  rgba(229, 231, 235, 0.5) 0.05%,
  rgba(229, 231, 235, 0) 25.05%
);
```

## Instruction

1. Create HTML Structure:

- Define a form with three steps, each step in a separate div with a class of step.
- Include navigation buttons (Next, Previous, Confirm) in each step.

2. Add CSS Styling:

- Style the form and steps to be visually appealing.
- Use CSS to hide all steps except the current one.

3. Implement JavaScript:

- Write JavaScript to handle showing and hiding steps.
- Add event listeners to navigation buttons to move between steps.
- Handle form submission to show a success message.

### JavaScript Example

Here is an example of how you can implement a music player app using vanilla JavaScript.

```javascript
// script.js
let currentStep = 1;

function showStep(step) {
  // Display current step in the UI
}

function nextStep() {
  // Handle next step function
}

function prevStep() {
  // Handle previous step function
}

document
  .getElementById("multiStepForm")
  .addEventListener("submit", function (event) {
    event.preventDefault();
    alert("🎉 Success");
  });

showStep(currentStep);
```

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
