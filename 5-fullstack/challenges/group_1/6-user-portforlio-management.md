---
title: "User Portfolio Management"
description: "In this challenge, you will develop a full-stack application that allows users to sign up and create/manage their developer portfolios. The focus will be on implementing robust user data management, ensuring security, creating dynamically generated pages, and optimizing the app for search engines (SEO)."
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
  - Create a User Portfolio Management App according to the design.
  - By default, users are asked to sign in.
  - On 'Sign In' Page, users can choose login with Github or by email and password.
  - On 'Sign In' Page, users can select the 'forgot password' option and be redirected to the 'Forgot password' page.
  - On 'Forgot Password' page, user can enter their email and get a magic link after selecting the 'Reset Password' button.
  - When users select the magic link, they are redirected to the 'Choose new password' page.
  - On 'Choose new password' page, users can enter a new password with the requirements given in the design.
  - Users can sign up with email and password. Optionally, an email with a magic link can be sent to verify the account.
  - On 'Profile setting' page, logged-in users can update their profile image, job title, name, and bio.
  - On 'Projects setting' page, logged-in users can add new projects with project name, demo URL, repository URL, and description.
  - On 'Projects setting' page, logged-in users can edit added projects.
  - On 'Portfolio' page, users can see the name, job title, bio, and the projects.
  - On 'Portfolio' page, others can send the user an email by selecting the contact button.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "User Portfolio Management | Full-stack project"
  description: "In this challenge, you will develop a full-stack application that allows users to sign up and create/manage their developer portfolios. The focus will be on implementing robust user data management, ensuring security, creating dynamically generated pages, and optimizing the app for search engines (SEO)."
  keywords:
    - "react"
    - "front-end libraries"
    - "full-stack"
challengeTexts:
  - Easy Portfolio for Developer
  - As a web developer, having a portfolio is essential for showcasing your technical skills and attracting potential clients. A portfolio is a museum of your work, with past tech stacks, case studies, and your work history.
  - Login to account
  - Enter your credentials to access your account
  - Sign in with Github
  - Enter email
  - Enter a password
  - Forgot password
  - Not a member?
  - Create an account
  - Create your account
  - Enter the fields below to get started
  - one lowercase character
  - one special character
  - one uppercase character
  - 8 character minimum
  - one number
  - Already have an account?  Log in
  - We’ll email you instructions to reset your password
  - Back to login
  - Choose a new password
  - Enter your new password and you’re all set.
  - Re-enter a password
  - Profile settings
  - Image must be 256 x 256px - max 2MB
  - Upload Profile Image
  - Delete Image
  - Job title
  - example@mail.com
  - Enter your job title
  - Enter your name
  - Enter a short introduction..
  - Projects settings
  - Add project
  - Image must be PNG or JPEG - max 2MB
  - Project Name
  - Enter your project name
  - Demo URL
  - Enter the demo URL
  - Repository URL
  - Enter the repository URL
  - Enter a short description..
  - A passionate Junior Front-end Developer with extensive experience in HTML, CSS, JavaScript, and React. Proven track record of developing user-friendly interfaces and optimizing website performance. Eager to learn and grow in the tech industry.
---

## Learning Goals

By completing this challenge, you will:

- Gain experience in full-stack development by creating a User Portfolio Management App.
- Enable users to sign up and create/manage their developer portfolios.
- Implement robust user data management and ensure security.
- Create dynamically generated pages for user profiles and projects.
- Optimize the app for search engines (SEO).
- Enhance your skills in front-end development using React, JavaScript, and CSS.
- Improve your understanding of server-side development using Node.js.
- Gain experience in deploying web applications and submitting repository and demo URLs.

## Requirements

You should create a web application that includes the following elements:

- Create a User Portfolio Management App according to the design.
- By default, users are asked to sign in.
- On 'Sign In' Page, users can choose login with Github or by email and password.
- On 'Sign In' Page, users can select the 'forgot password' option and be redirected to the 'Forgot password' page.
- On 'Forgot Password' page, user can enter their email and get a magic link after selecting the 'Reset Password' button.
- When users select the magic link, they are redirected to the 'Choose new password' page.
- On 'Choose new password' page, users can enter a new password with the requirements given in the design.
- Users can sign up with email and password. Optionally, an email with a magic link can be sent to verify the account.
- On 'Profile setting' page, logged-in users can update their profile image, job title, name, and bio.
- On 'Projects setting' page, logged-in users can add new projects with project name, demo URL, repository URL, and description.
- On 'Projects setting' page, logged-in users can edit added projects.
- On 'Portfolio' page, users can see the name, job title, bio, and the projects.
- On 'Portfolio' page, others can send the user an email by selecting the contact button.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

### Front-end Development

1. **Framework**: Use React for building the user interface.
2. **State Management**: Use a state management tool like Zustand or Redux for managing state.
3. **Styling**: Use CSS-in-JS libraries like styled-components, tailwind, or traditional CSS for styling.

### Back-end Development

1. **Framework**: Use Node.js with Express.js or Next.js to create the server.
2. **Database**: Use a database of your choice (e.g., MongoDB or PostgreSQL) for storing user data.

### Authentication

- **Required**: Users should be able to log in with Github or by email and password.

### Password Reset

- **Required**: Users should be able to reset their password using a magic link sent to their email.

### API Integration

**Email Service API**

You can use an email service API (e.g., SendGrid) to send emails for password reset and account verification.

**Custom API**

- Create User: Endpoint to create a new user account.
- Update User: Endpoint to update user profile and project details.
- Get User: Endpoint to fetch user profile and project details.
- Send Email: Endpoint to send emails for password reset and account verification.

**API Endpoints**

1. **POST /api/user/signup**: Create a new user account.
2. **POST /api/user/login**: Log in with email and password.
3. **POST /api/user/login/github**: Log in with Github.
4. **POST /api/user/forgot-password**: Send a magic link to reset the password.
5. **POST /api/user/reset-password**: Reset the password using the magic link.
6. **PUT /api/user/profile**: Update user profile details.
7. **PUT /api/user/projects**: Add or edit user projects.
8. **GET /api/user/profile**: Fetch user profile details.
9. **GET /api/user/projects**: Fetch user projects.

### Deployment

1. Front-end: Deploy the React app on Netlify or Vercel.
2. Back-end: Deploy the Node.js server on Heroku, AWS, or Vercel.

Submit the repository URL and demo URL after deployment.
