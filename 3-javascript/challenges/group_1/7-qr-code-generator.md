---
title: "QR Code Generator App - QRCODE"
description: "This challenge provides an excellent opportunity to practice your JavaScript skills by creating a simple QR code generator application that requires the use of an external library."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "HTML"
  - "CSS"
  - "JavaScript"
lessons:
  - 3-javascript/javascript-modules-basics
  - 3-javascript/javascript-dom-and-events
userStories:
  - Create a QR code generator app that matches the given design.
  - Use HTML to create the basic structure.
  - Add inputs, buttons,.. according to the design.
  - Use vanilla JavaScript to add interactivity.
  - Users can enter a URL.
  - User can see a QR quote after selecting the QR code button.
  - User can download QR quote image by selecting download button.
  - User can copy Quote to the clipboard by selecting Share button.
  - The page should be responsive on different screen sizes.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "QR Code Generator App - QACODE"
  description: "This challenge provides an excellent opportunity to practice your JavaScript skills by creating a simple QR code generator application that requires the use of an external library. Enhance your JavaScript skills and gain experience in utilizing external libraries by creating a QR code generator app. This project will help you practice HTML, CSS, and JavaScript, as well as improve your ability to create interactive web applications. By deploying the solution and submitting the Repository URL and Demo URL, you will showcase your work to others."
  keywords:
    - "qr code generator app"
    - "html css javascript"
challengeTexts:
  - Enter an url
  - Download
  - Share
---

## Learning Goals

By completing this challenge, you will:

- Practice your JavaScript skills by creating a simple QR code generator application.
- Learn how to create a QR code generator app that matches a given design.
- Improve your HTML, CSS, and JavaScript skills.
- Enhance your ability to create interactive web applications.

## Requirements

You should create a web page that includes the following elements:

- Create a QR code generator app that matches the given design.
- Use HTML to create the basic structure.
- Add inputs, buttons,.. according to the design.
- Use vanilla JavaScript to add interactivity.
- Users can enter a URL.
- User can see a QR quote after selecting the QR code button.
- User can download QR quote image by selecting download button.
- User can copy Quote to the clipboard by selecting Share button.
- Ensure the page is responsive on different screen sizes.
- Deploy the solution and submit both the Repository URL and Demo URL.

## Technical Details

To generate QR codes for this challenge, you can use the `qrcodejs` library. You can include the library in your HTML file by adding the following script tag:

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
```

Once the library is included, you can use it to generate QR codes by creating a new instance of the `QRCode` class and passing the target element and the data you want to encode. Here's an example:

```javascript
const qrCode = new QRCode(document.getElementById("qrcode"), {
  text: "https://example.com",
  width: 128,
  height: 128,
});
```

In this example, the QR code will be generated inside the element with the ID "qrcode" and will encode the URL "https://example.com". You can customize the width and height of the QR code as needed.

Remember to include the necessary HTML elements and CSS styles to create the QR code generator app according to the given design.

## Instructions

To complete this challenge, you can follow these steps:

1. Set up the basic structure of the HTML document.
2. Create a container element to hold the QR code and input field.
3. Use CSS to style the container element according to the given design.
4. Add an input field for users to enter a URL.
5. Create a button element for generating the QR code.
6. Use the `qrcodejs` library to generate the QR code based on the entered URL.
7. Implement the functionality to download the QR code image when the download button is clicked.
8. Implement the functionality to copy the QR code to the clipboard when the share button is clicked.
9. Ensure that the page is responsive by using CSS media queries.
10. Test your application to make sure it works as expected.
11. Deploy your solution to a hosting platform of your choice.
12. Submit the Repository URL and Demo URL for evaluation.

Good luck with the challenge!

### JavaScript Instruction

1. Include the `qrcodejs` library:

- Add the following script tag to your HTML file to include the `qrcodejs` library:

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
```

2. Generate the QR code:

- Create a new instance of the `QRCode` class and pass the target element and the data you want to encode. Here's an example:

```javascript
const qrCode = new QRCode(document.getElementById("qrcode"), {
  text: "https://example.com",
  width: 128,
  height: 128,
});
```

- Customize the `text`, `width`, and `height` properties of the `QRCode` instance as needed.

3. Download the QR code:

- Implement the functionality to download the QR code image when the download button is clicked. You can use the `download` attribute of an `<a>` element to achieve this.

4. Copy the QR code to the clipboard:

- Implement the functionality to copy the QR code to the clipboard when the share button is clicked. You can use the `execCommand('copy')` method to copy the text to the clipboard.

Remember to include the necessary HTML elements and CSS styles to create the QR code generator app according to the given design.

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.

## Tech Stack

For this project, it is recommended to use HTML, CSS, and JavaScript to create the web page. You can use any text editor or integrated development environment (IDE) to write your code. There are no specific requirements for the choice of HTML, CSS, and JavaScript frameworks or libraries. It is recommended to use Vanilla JavaScript for this project.
