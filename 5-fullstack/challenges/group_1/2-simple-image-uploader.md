---
title: "Simple Image Upload App"
description: "In full-stack development, a common task involves working with files. This challenge presents an opportunity to create a straightforward Image Upload application, enabling users to upload images."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - React
  - JavaScript
  - NodeJs
lessons:
  - 1-fundamentals/free-hosting-for-web-projects
userStories:
  - Create a simple image upload application following the given design.
  - Users can upload an image at a time. The file should be JPG, PNG, or GIF. The maximum size is 2MB.
  - Users can drag and drop the file to upload it.
  - Users can browse files and select a file to upload.
  - When the image is uploading, users can see a loader like in the design.
  - When the image is successfully uploaded, users can see the image.
  - After the image is uploaded, users can copy its address by selecting the `Share` button.
  - After the image is uploaded, users can download the image by selecting the `Download` button.
  - Optionally, users can change the theme between dark and light.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Simple Image Upload App | Full-stack project"
  description: "In full-stack development, a common task involves working with files. This challenge presents an opportunity to create a straightforward Image Upload application, enabling users to upload images."
  keywords:
    - "react"
    - "front-end libraries"
    - "full-stack"
challengeTexts:
  - Drag & drop a file or browse files
  - JPG, PNG or GIF - Max file size 2MB
  - Uploading, please wait..
  - Share
  - Download
---

## Learning Goals

By completing this challenge, you will:

- Gain experience in full-stack development by creating a Simple Image Upload App.
- Implement the ability for users to upload images and view them.
- Learn how to handle file uploads and validate file types and sizes.
- Enhance your skills in front-end development using React, HTML, CSS, and JavaScript.
- Improve your understanding of responsive web design and creating applications that work well on all devices.
- Gain experience in deploying web applications and submitting repository and demo URLs.

## Requirements

You should create a web page that includes the following elements:

- Create a simple image upload application following the given design.
- Users can upload an image at a time. The file should be JPG, PNG, or GIF. The maximum size is 2MB.
- Users can drag and drop the file to upload it.
- Users can browse files and select a file to upload.
- When the image is uploading, users can see a loader like in the design.
- When the image is successfully uploaded, users can see the image.
- After the image is uploaded, users can copy its address by selecting the `Share` button.
- After the image is uploaded, users can download the image by selecting the `Download` button.
- Optionally, users can change the theme between dark and light.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

### Front-end Development

1. **Framework**: Use React for building the user interface.
2. **File Upload**: Use the `react-dropzone` library for drag-and-drop file upload functionality.
3. **State Management**: Use React's `useState` and `useEffect` hooks for managing state.
4. **Styling**: Use CSS-in-JS libraries like styled-components, tailwind or traditional CSS for styling.

### Back-end Development

1. **Framework**: Use Node.js with Express.js to create the server.
2. **File Storage**: Use a cloud storage service like AWS S3 or a local storage solution for storing uploaded images.
3. **File Validation**: Validate file type and size on the server-side before saving.
4. **API Endpoints**:

- POST /api/upload: Handle image upload and return the image URL.
- GET /api/download/:filename: Handle image download.

**Deployment**

1. Front-end: Deploy the React app on Netlify or Vercel.
2. Back-end: Deploy the Node.js server on Heroku/AWS or Vercel.

Submit the repository URL and demo URL after deployment.
