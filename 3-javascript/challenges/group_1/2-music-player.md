---
title: "Music Player"
description: "This challenge is an excellent opportunity to enhance your JavaScript skills by creating a simple music player app that tests your data management capabilities using JavaScript."
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
  - Create a music player app that matches the given design.
  - Use HTML to create the basic structure, including elements such as image, title, author, progress bar, and player button.
  - Implement interactivity using vanilla JavaScript.
  - Allow users to play and stop the current song.
  - Enable navigation to next and previous songs.
  - Allow users to change play time using the progress bar.
  - Ensure the page is responsive on different screen sizes.
  - Deploy the solution and provide the Repository URL and Demo URL.
seo:
  title: "Music Player App"
  description: "Create a simple music player app using HTML, CSS, and JavaScript. Enhance your JavaScript skills and test your data management capabilities. This project will help you practice HTML, CSS, and JavaScript, as well as improve your ability to create interactive web applications. By deploying the solution and submitting the Repository URL and Demo URL, you will gain experience in sharing your work with others."
  keywords:
    - "music player app challenge"
    - "html css javascript"
challengeTexts:
  - Lost in the City Lights
  - Cosmo Sheldrake
  - Forest Lullaby
  - Lesfm
---

## Goals

By completing this challenge, you will:

- Improve your HTML, CSS, and JavaScript skills.
- Enhance your ability to create interactive web applications.
- Implement interactivity using vanilla JavaScript.
- Gain experience in data management using JavaScript.

## Requirements

You should create a web page that includes the following elements:

- A music player app that matches the given design
- HTML structure for the basic elements such as image, title, author, progress bar, player button, etc.
- Use vanilla JavaScript to add interactivity
- Users should be able to play and stop the current song
- Users should be able to go to next and previous songs
- Users should be able to change play time with the progress bar
- The page should be responsive on different screen sizes
- Deploy the solution and submit Repository URL and Demo URL

## Technical Details

You can use the provided shadow values or customize it with your own values.

```css
/* Play Button shadow */
filter: drop-shadow(0px 8px 16px rgba(201, 59, 118, 0.25));
```

## Instruction

To add a music player app with vanilla JavaScript, follow these steps:

1. Create the basic structure of the music player app using HTML. Include elements such as an image, title, author, progress bar, and player button.
2. Use CSS to style the music player app according to the given design. You can customize the provided shadow values or use your own.
3. Implement interactivity using vanilla JavaScript. Add event listeners to the player button and progress bar to handle play, stop, next, previous, and play time change functionalities.
4. Use JavaScript to manage the data of the music player app. You can store the song information in an array or object and update the UI accordingly.
5. Test the music player app by playing, stopping, navigating between songs, and changing the play time using the progress bar.
6. Ensure that the music player app is responsive on different screen sizes. Use CSS media queries to adjust the layout and styling as needed.
7. Deploy the solution to a hosting platform of your choice. Provide the Repository URL and Demo URL when submitting your solution.

Remember to test your app thoroughly and handle any edge cases or errors that may occur during usage.

### JavaScript Instructions for Music Player

1. Create HTML Structure:

- Add audio controls, play/pause button, and progress bar.

2. Select DOM Elements:

- Use `document.getElementById` or `document.querySelector` to select the necessary elements.

3. Add Event Listeners:

- Add event listeners for play/pause button and progress bar.

4. Update Progress Bar:

- Write a function to update the progress bar as the audio plays.

5. Seek Functionality:

- Implement functionality to seek to different parts of the audio using the progress bar.

Here is an example of how you can implement a music player app using vanilla JavaScript:

```javascript
// script.js

const songs = [
  {
    title: "Song 1",
    author: "Artist 1",
    src: "song1.mp3",
    img: "cover1.jpg",
  },
  {
    title: "Song 2",
    author: "Artist 2",
    src: "song2.mp3",
    img: "cover2.jpg",
  },
];

let currentSongIndex = 0;
const audio = new Audio(songs[currentSongIndex].src);

document.getElementById("playButton").addEventListener("click", playPause);
document.getElementById("nextButton").addEventListener("click", nextSong);
document.getElementById("prevButton").addEventListener("click", prevSong);
audio.addEventListener("timeupdate", updateProgressBar);

function playPause() {
  // Add pause button implementation
}

function nextSong() {
  // Add next button implementation
}

function prevSong() {
  // Add previous button implementation
}

function loadSong(index) {
  // Add load song implementation
}

function updateProgressBar() {
  // Handle when progress bar is updated
}

document.getElementById("progressBar").addEventListener("input", function () {
  audio.currentTime = (this.value / 100) * audio.duration;
});

// Initial load
loadSong(currentSongIndex);
```

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
