---
title: "Text to Speech - Speechbot"
description: "The challenge is to create a simple text-to-speech application using advanced built-in JavaScript functionality. This involves working with JavaScript APIs such as the Speech Recognition API and the Speech Synthesis API."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/javascript-oop-concepts
  - 3-javascript/javascript-dom-and-events
userStories:
  - Create a text-to-speech app that matches the given design.
  - Use HTML to create the basic structure.
  - Add inputs, tabs, buttons,.. according to the design.
  - Use JavaScript to add interactivity.
  - Users can enter custom text.
  - Users can choose the voice of the speech, the default should be 'Albert'.
  - Users can choose the speed of the speech (0.5, 0.75, 1 or 1.5 times).
  - Users can select Text to Speech button and listen to the speech.
  - The page should be responsive on different screen sizes.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Text to Speech - Speechbot"
  description: "The challenge is to create a simple text-to-speech application using advanced built-in JavaScript functionality. This involves working with JavaScript APIs such as the Speech Recognition API and the Speech Synthesis API. Create a text-to-speech app that matches the given design. Use HTML to create the basic structure. Add inputs, tabs, buttons,.. according to the design. Use JavaScript to add interactivity. Users can enter custom text. Users can choose the voice of the speech, the default should be 'Albert'. Users can choose the speed of the speech (0.5, 0.75, 1 or 1.5 times). Users can select Text to Speech button and listen to the speech. The page should be responsive on different screen sizes. Deploy the solution and submit Repository URL and Demo URL."
  keywords:
    - "text to speech challenge"
    - "html css javascript"
challengeTexts:
  - Enter your text
  - Enter your text above and hit 'play.' You can choose a different voice by selecting an option from the dropdown menu.
---

## Learning Goals

The goals of this project are to help you:

- Gain practical experience in utilizing external APIs within your application
- Practice vanilla JavaScript, CSS, and HTML
- Develop a text-to-speech application using advanced built-in JavaScript functionality
- Work with JavaScript APIs such as the Speech Recognition API and the Speech Synthesis API
- Create a responsive web page that is functional on different screen sizes

## Requirements

The goals of this project are to help you:

- Create a text-to-speech app that matches the given design.
- Use HTML to create the basic structure.
- Add inputs, tabs, buttons,.. according to the design.
- Use JavaScript to add interactivity.
- Users can enter custom text.
- Users can choose the voice of the speech, the default should be 'Albert'.
- Users can choose the speed of the speech (0.5, 0.75, 1 or 1.5 times).
- Users can select Text to Speech button and listen to the speech.
- The page should be responsive on different screen sizes.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

- You can use the provided shadow values or customize it with your own values.

```css
background: linear-gradient(91deg, #6326a2 1.16%, #263fa9 100%);

box-shadow: 0px 4px 8px 0px rgba(28, 27, 67, 0.3);
```

- Use the Speech Recognition API to recognize user speech input.

```javascript
// Speech Recognition API
const recognition = new SpeechRecognition();
```

- Use the Speech Synthesis API to convert text to speech.

```javascript
// Speech Synthesis API
const synthesis = window.speechSynthesis;
```

## Instructions

To complete this challenge, you can follow these steps:

1. Set up the basic structure of the HTML document.
2. Create input elements for users to enter custom text.
3. Add a dropdown menu for users to choose the voice of the speech.
4. Add a dropdown menu for users to choose the speed of the speech.
5. Implement JavaScript functionality to convert text to speech using the selected voice and speed.
6. Add event listeners to the Text to Speech button to trigger the speech synthesis.
7. Ensure that the page is responsive by using CSS media queries.
8. Test your application to make sure it works as expected.
9. Deploy your solution to a hosting platform of your choice.
10. Submit the Repository URL and Demo URL for evaluation.

Good luck with the challenge!

### JavaScript Instruction

1. Recognize User Speech Input:

- Use the Speech Recognition API to recognize user speech input.

2. Convert Text to Speech:

- Use the Speech Synthesis API to convert text to speech.

3. Add Event Listener for Text to Speech Button:

- Add an event listener to the Text to Speech button to trigger the speech synthesis.

```javascript
// Speech Recognition API
const recognition = new SpeechRecognition();

// Speech Synthesis API
const synthesis = window.speechSynthesis;

// Recognize user speech input
recognition.addEventListener("result", (event) => {
  // Handle recognized speech input
});

// Convert text to speech
function convertTextToSpeech(text, voice, speed) {
  // Implement text to speech functionality
}

// Add event listener to Text to Speech button
document.getElementById("textToSpeechButton").addEventListener("click", () => {
  // Get user input values
  const text = document.getElementById("textInput").value;
  const voice = document.getElementById("voiceSelect").value;
  const speed = document.getElementById("speedSelect").value;

  // Convert text to speech
  convertTextToSpeech(text, voice, speed);
});
```

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
