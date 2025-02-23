---
title: "My Task Board"
description: "In this full-stack challenge, you will develop a straightforward task management application, which will involve implementing essential HTTP methods such as GET, POST, PUT, and DELETE. This project will provide an opportunity to demonstrate proficiency in full-stack development by creating a system that enables users to manage tasks using a range of fundamental HTTP operations."
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
  - Create a simple task management application following the given design.
  - By default, it should show a board with 4 tasks like in the design.
  - Users can edit task name, description, icon, and status.
  - Users can delete tasks by selecting `Delete` button.
  - When users select `Add new task` option, a new task is added with a default name.
  - Users can edit board name and optionally, users can edit board description as well.
  - When users first visit the app, a new board with a unique id is created and saved to the database or alternatively a board is created after users make the first change.
  - "Each board can be accessed by a unique id, e.g: /board/:board-id"
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "My Task Board | Full-stack project"
  description: "In this full-stack challenge, you will develop a straightforward task management application, which will involve implementing essential HTTP methods such as GET, POST, PUT, and DELETE. This project will provide an opportunity to demonstrate proficiency in full-stack development by creating a system that enables users to manage tasks using a range of fundamental HTTP operations."
  keywords:
    - "react"
    - "front-end libraries"
    - "full-stack"
challengeTexts:
  - My Task Board
  - Tasks to keep organised
  - Enter a short description
  - In Progress
  - Completed
  - Won’t do
  - Task in Progress
  - Task Completed
  - Task Won’t Do
  - Task To Do
  - Add new task
---

## Learning Goals

By completing this challenge, you will:

- Gain experience in full-stack development by creating a simple task management application.
- Implement essential HTTP methods such as GET, POST, PUT, and DELETE.
- Demonstrate proficiency in full-stack development by creating a system that enables users to manage tasks using a range of fundamental HTTP operations.
- Enhance your skills in front-end development using React, JavaScript, and CSS.
- Improve your understanding of database operations and server-side development using Node.js.
- Gain experience in deploying web applications and submitting repository and demo URLs.

## Requirements

You should create a web page that includes the following elements:

- Create a simple task management application following the given design.
- By default, it should show a board with 4 tasks like in the design.
- Users can edit task name, description, icon, and status.
- Users can delete tasks by selecting `Delete` button.
- When users select `Add new task` option, a new task is added with a default name.
- Users can edit board name and optionally, users can edit board description as well.
- When users first visit the app, a new board with a unique id is created and saved to the database or alternatively a board is created after users make the first change.
- Each board can be accessed by a unique id, e.g: /board/:board-id
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

### Front-end Development

1. **Framework**: Use React for building the user interface.
2. **State Management**: Use a state management tool like Zustand or Redux for managing state.
3. **Styling**: Use CSS-in-JS libraries like styled-components, tailwind or traditional CSS for styling.

### Back-end Development

1. **Framework**: Use Node.js with Express.js or Next.js to create the server.
2. **Database**: Use a database of your choice (e.g., MongoDB or PostgreSQL) for storing tasks and boards.

### API Endpoints

1. **GET /api/boards/:board-id**: Retrieve a board by its ID.
2. **POST /api/boards**: Create a new board and return the generated ID.
3. **PUT /api/boards/:board-id**: Update a board by its ID.
4. **DELETE /api/boards/:board-id**: Delete a board by its ID.
5. **PUT /api/tasks/:task-id**: Update a task by its ID.
6. **DELETE /api/tasks/:task-id**: Delete a task by its ID.

### Default Task Board

- By default, the task board should have the following columns: "In Progress", "Completed", and "Won't do".
- Each column should have a default task: "Task in Progress", "Task Completed", and "Task Won't Do".
- Users can edit the task name, description, icon, and status.

### Add New Task Functionality

- When users select the "Add new task" option, a new task is added with a default name.
- Users can edit the task name, description, icon, and status.

### Board Management

- Users can edit the board name and optionally, the board description.
- When users first visit the app, a new board with a unique id is created and saved to the database. Alternatively, a board is created after users make the first change.
- Each board can be accessed by a unique id, e.g: /board/:board-id.

### Deployment

1. Front-end: Deploy the React app on Netlify or Vercel.
2. Back-end: Deploy the Node.js server on Heroku, AWS, or Vercel.

Submit the repository URL and demo URL after deployment.
