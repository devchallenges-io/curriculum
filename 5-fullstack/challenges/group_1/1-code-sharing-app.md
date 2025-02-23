---
title: "Code Sharing App - NoteCode"
description: "This challenge is an excellent opportunity for Fullstack developers to test their basic skills by creating a simple code-sharing application called NoteCode. The application will allow users to store and share coding snippets, and it will require the use of both front-end and back-end development skills."
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
  - Create a Coding Sharing App - NoteCode following given design.
  - By default, users should see an HTML given snippet. See `Code Guide` for default HTML code.
  - When users select the `Share` button, a new ID should be generated, and users can access the saved code with the generated ID. See `Code Guide` for more details.
  - After code is saved and shared, `Share` button should be disabled until users make an edit .
  - Users can choose the language and theme they want to save and share.
  - The application should be responsive on all devices.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "Code Sharing App - NoteCode| Full-stack project"
  description: "This challenge is an excellent opportunity for Fullstack developers to test their basic skills by creating a simple code-sharing application called NoteCode. The application will allow users to store and share coding snippets, and it will require the use of both front-end and back-end development skills."
  keywords:
    - "react"
    - "front-end libraries"
    - "full-stack"
challengeTexts:
  - Create & Share
  - Your Code easily
---

## Learning Goals

By completing this challenge, you will:

- Gain experience in full-stack development by creating a Code Sharing App - NoteCode.
- Implement the ability for users to create, save, and share coding snippets.
- Learn how to generate unique IDs for saved code snippets.
- Enhance your skills in front-end development using HTML, CSS, and JavaScript.
- Improve your understanding of responsive web design and creating applications that work well on all devices.
- Gain experience in deploying web applications and submitting repository and demo URLs.

## Requirements

You should create a web page that includes the following elements:

- Create a Coding Sharing App - NoteCode following given design.
- By default, users should see an HTML given snippet. See `Code Guide` for default HTML code.
- When users select the `Share` button, a new ID should be generated, and users can access the saved code with the generated ID. See `Code Guide` for more details.
- After code is saved and shared, `Share` button should be disabled until users make an edit .
- Users can choose the language and theme they want to save and share.
- The application should be responsive on all devices.
- User authentication is not required
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

### Front-end Development

1. **Framework**: Use React for building the user interface.
2. **Code Editor**: Integrate [monaco-editor](https://microsoft.github.io/monaco-editor/) or CodeMirror or Ace Editor for the code editing functionality.
3. **State Management**: Use React's useState and useEffect hooks for managing state.
4. **Styling**: Use CSS-in-JS libraries like styled-components, tailwind or traditional CSS for styling.
5. **Responsive Design**: Implement responsive design using CSS media queries and Flexbox/Grid layout.

### Back-end Development

1. **Framework**: Use Node.js with Express.js or Next.js to create the server.
2. **Database**: Users can choose any database of their preference for storing the code snippets. Some popular options include: MongoDB or PostgreSQL.
3. **ID Generation**: Use a library like uuid to generate unique IDs for each code snippet.

### API Endpoints

1. **POST /api/snippets**: Save a new code snippet and return the generated ID.
2. **GET /api/snippets/:id**: Retrieve a code snippet by its ID.

### Default HTML Snippet

- Store the default HTML snippet in a constant and load it into the editor on initial render.

```html
<html>
  <head>
    <title>HTML Sample</title>
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <style type="text/css">
      h1 {
        color: #cca3a3;
      }
    </style>
    <script type="text/javascript">
      alert("I am a sample... visit devChallengs.io for more projects");
    </script>
  </head>
  <body>
    <h1>Heading No.1</h1>
    <input disabled type="button" value="Click me" />
  </body>
</html>
```

### Share Button Functionality

1. Initial State: The Share button is enabled.
2. On Share: Generate a new ID, save the code snippet, and disable the Share button.
3. On Edit: Re-enable the Share button when the user makes an edit.

### Deployment

1. Front-end: Deploy the React app on Netlify or Vercel.
2. Back-end: Deploy the Node.js server on Heroku/AWS or Vercel.

Submit the repository URL and demo URL after deployment.
