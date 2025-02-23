---
title: "AI Image Generation App"
description: "The challenge is to create a full-stack application that allows users to generate AI images, manage their own collections, and view others' generated images. The fusion of AI and full-stack development opens doors to a future where web applications are more responsive and capable than ever before."
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
  - Create an Image Generation App according to the design.
  - By default, the active tab should be 'Generate Image' page.
  - Users can log in with Github or your chosen third party.
  - On Generate Image page, users can enter a prompt, enter a negative prompt, select a color, select a resolution, and change guidance.
  - Given a valid prompt and a logged-in user, they can generate a new image by selecting the 'Generate Image' button.
  - On Feed page, users can see a list of cards. Each card includes a generated image, author name, and a bookmark button.
  - On Feed page, users can search images by keywords. Keywords are from generated prompts.
  - On Feed page, users can save images to their collection.
  - On Feed page, users can select a card and see the image details.
  - On Image details modal, users can see the generated image, the prompt, the negative prompt, created date, resolution, and seed number.
  - On Image details modal, users can copy the settings to generate a new image by selecting the 'Generate with this settings' button.
  - On Image details modal, users can download the image.
  - On Generation History Page, users can see their generated image history.
  - On My Collection Page, users see the saved images.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "AI Image Generation App | Full-stack project"
  description: "The challenge is to create a full-stack application that allows users to generate AI images, manage their own collections, and view others' generated images. The fusion of AI and full-stack development opens doors to a future where web applications are more responsive and capable than ever before."
  keywords:
    - "react"
    - "front-end libraries"
    - "full-stack"
challengeTexts:
  - Enter the prompt
  - Negative Prompt (Optional)
  - Resolution
  - Guidance (5.0)
  - Generate Image
  - Breathtaking digital art illustration of a celestial galaxy, bursting with vibrant colors and sparkling stars, reminiscent of an infinite cosmic journey
  - Search images by keywords
  - Generation History
  - Prompt details
  - Negative prompt
  - Created on
  - Input Resolution
  - My Collection
  - Generate with this settings
  - Sign In to Continue
  - Sign in with Github
---

## Learning Goals

By completing this challenge, you will:

- Gain experience in full-stack development by creating an AI Image Generation App.
- Enable users to generate AI images, manage their own collections, and view others' generated images.
- Implement functionality for users to enter prompts, select colors and resolutions, and change guidance.
- Enhance your skills in front-end development using React, JavaScript, and CSS.
- Improve your understanding of server-side development using Node.js.
- Gain experience in deploying web applications and submitting repository and demo URLs.

## Requirements

You should create a web application that includes the following elements:

- Create an Image Generation App according to the design.
- By default, the active tab should be the 'Generate Image' page.
- Users can log in with Github or your chosen third party.
- On the Generate Image page, users can enter a prompt, enter a negative prompt, select a color, select a resolution, and change guidance.
- Given a valid prompt and a logged-in user, they can generate a new image by selecting the 'Generate Image' button.
- On the Feed page, users can see a list of cards. Each card includes a generated image, author name, and a bookmark button.
- On the Feed page, users can search images by keywords. Keywords are from generated prompts.
- On the Feed page, users can save images to their collection.
- On the Feed page, users can select a card and see the image details.
- On the Image details modal, users can see the generated image, the prompt, the negative prompt, created date, resolution, and seed number.
- On the Image details modal, users can copy the settings to generate a new image by selecting the 'Generate with this settings' button.
- On the Image details modal, users can download the image.
- On the Generation History Page, users can see their generated image history.
- On the My Collection Page, users see the saved images.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

### Front-end Development

1. **Framework**: Use React for building the user interface.
2. **State Management**: Use a state management tool like Zustand or Redux for managing state.
3. **Styling**: Use CSS-in-JS libraries like styled-components, tailwind, or traditional CSS for styling.

### Back-end Development

1. **Framework**: Use Node.js with Express.js or Next.js to create the server.
2. **Database**: Use a database of your choice (e.g., MongoDB or PostgreSQL) for storing collections.

### Authentication

- **Required**: Users should be able to log in with Github or your chosen third party.

### API Integration

**AI Image Generation API**

You can use OpenAI or similar APIs for generating AI images.

**Custom API**

- Create Collection: Endpoint to create a new collection.
- Get Collections: Endpoint to fetch all collections.
- Save Image to Collection: Endpoint to save an image to a collection.
- Get Image Details: Endpoint to fetch details of a specific image.
- Get Generation History: Endpoint to fetch the user's generated image history.
- Get My Collection: Endpoint to fetch the user's saved images.

**API Endpoints**

1. **POST /api/generate**: Generate an AI image based on user prompts.
2. **GET /api/feed**: Retrieve a list of generated images for the feed page.
3. **GET /api/feed/search**: Search generated images by keywords.
4. **POST /api/feed/save**: Save an image to the user's collection.
5. **GET /api/image/:image-id**: Retrieve details of a specific image.
6. **POST /api/image/:image-id/generate**: Generate a new image with the same settings as the selected image.
7. **GET /api/history**: Retrieve the user's generated image history.
8. **GET /api/collection**: Retrieve the user's saved images.

### Deployment

1. Front-end: Deploy the React app on Netlify or Vercel.
2. Back-end: Deploy the Node.js server on Heroku, AWS, or Vercel.

Submit the repository URL and demo URL after deployment.
