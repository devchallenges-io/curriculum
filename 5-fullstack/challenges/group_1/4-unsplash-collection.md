---
title: "Unsplash Collection - Unsplash Box"
description: "In this full-stack challenge, you will develop a service to store collections of Unsplash images, allowing users to add Unsplash images to their collections. This project will involve creating a functionality similar to Unsplash's collection feature, providing an opportunity to demonstrate proficiency in full-stack development by enabling users to manage and store curated sets of Unsplash images."
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
  - Create a multiple-page website following the given design.
  - On Homepage, users can search for images from Unsplash given keywords.
  - On Homepage, when user press `Enter`, a list of images should be shown as a result if at least a keyword is provided.
  - Users can select an image and see its details in a separate Image page.
  - On Image page, users can see the author and published date.
  - On Image page, users can see a list of collections that the image belongs to.
  - On Image page, users can choose to add the image to a collection by selecting `Add to Collection` button.
  - When `Add to Collection` button is selected, users can search and add images to searched collections. The collection search result should only show collections that the image does not yet belong to.
  - On Image page, users can remove the image from its collections.
  - On Image page, users can download the image.
  - On Collections page, users can see and select existing collections.
  - On Collections page, when a collection is selected, users can see a list of images in the collection.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Unsplash Collection - Unsplash Box | Full-stack project"
  description: "In this full-stack challenge, you will develop a service to store collections of Unsplash images, allowing users to add Unsplash images to their collections. This project will involve creating a functionality similar to Unsplash's collection feature, providing an opportunity to demonstrate proficiency in full-stack development by enabling users to manage and store curated sets of Unsplash images."
  keywords:
    - "react"
    - "front-end libraries"
    - "full-stack"
challengeTexts:
  - Search high-resolution images from Unsplash
  - Enter your keywords...
  - Home
  - Explore the world through collections of beautiful photos free to use under the Unsplash License.
  - Add to Collection
  - Remove
  - Download
---

## Learning Goals

By completing this challenge, you will:

- Gain experience in full-stack development by creating a service to store collections of Unsplash images.
- Enable users to add Unsplash images to their collections and manage them.
- Implement functionality similar to Unsplash's collection feature.
- Demonstrate proficiency in full-stack development by creating a system that allows users to manage and store curated sets of Unsplash images.
- Enhance your skills in front-end development using React, JavaScript, and CSS.
- Improve your understanding of server-side development using Node.js.
- Gain experience in deploying web applications and submitting repository and demo URLs.

## Requirements

You should create a web page that includes the following elements:

- Create a multiple-page website following the given design.
- On the Homepage, users can search for images from Unsplash given keywords.
- On the Homepage, when the user presses `Enter`, a list of images should be shown as a result if at least one keyword is provided.
- Users can select an image and see its details in a separate Image page.
- On the Image page, users can see the author and published date.
- On the Image page, users can see a list of collections that the image belongs to.
- On the Image page, users can choose to add the image to a collection by selecting the `Add to Collection` button.
- When the `Add to Collection` button is selected, users can search and add images to searched collections. The collection search result should only show collections that the image does not yet belong to.
- On the Image page, users can remove the image from its collections.
- On the Image page, users can download the image.
- On the Collections page, users can see and select existing collections.
- On the Collections page, when a collection is selected, users can see a list of images in the collection.
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

- **Not Required**: Authentication is not required for this application. Users can access all features without logging in.

### API Integration

**Unsplash API**

- Search Images: Use the `/search/photos` endpoint to fetch images based on keywords.
- Image Details: Use the `/photos/:id` endpoint to fetch details of a specific image.

**Custom API**

- Create Collection: Endpoint to create a new collection.
- Get Collections: Endpoint to fetch all collections.
- Add Image to Collection: Endpoint to add an image to a collection.
- Remove Image from Collection: Endpoint to remove an image from a collection.
- Get Collection Images: Endpoint to fetch images in a specific collection.

**API Endpoints**

1. **GET /api/collections**: Retrieve a list of existing collections.
2. **GET /api/collections/:collection-id**: Retrieve details of a specific collection.
3. **POST /api/collections/:collection-id/images**: Add an image to a specific collection.
4. **DELETE /api/collections/:collection-id/images/:image-id**: Remove an image from a specific collection.
5. **GET /api/collections/:collection-id/images**: Retrieve a list of images in a specific collection.

### Deployment

1. Front-end: Deploy the React app on Netlify or Vercel.
2. Back-end: Deploy the Node.js server on Heroku, AWS, or Vercel.

Submit the repository URL and demo URL after deployment.
