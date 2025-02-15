---
title: "AI Chatbot - simplechat.ai"
description: "As AI is the future, knowing how to build an AI chatbot can be helpful. In this challenge, you will work with a provided API and build a simple AI chatbot."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "JavaScript"
  - "API Integration"
lessons:
  - 1-fundamentals/free-hosting-for-web-projects
userStories:
  - Create an AI chatbot that matches the given layout.
  - By default, users should see a small conversation between the user and the chatbot.
  - Users can ask the following questions and get responses from the chatbot.
  - Users can add new conversations. When a new conversation is added, its title should be the first question from the user.
  - Conversations should be stored in local storage.
  - Users can edit conversations' title.
  - Users can delete conversations.
  - The application should be responsive on all devices.
  - Deploy the solution and submit Repository URL and Demo URL.
seo:
  title: "AI Chatbot - simplechat.ai | Frontend, React project"
  description: "As AI is the future, knowing how to build an AI chatbot can be helpful. In this challenge, you will work with a provided API and build a simple AI chatbot. This project is great for working with Front-end libraries like React, Vue,..."
  keywords:
    - "AI chatbot"
    - "API integration"
    - "frontend developer"
challengeTexts:
  - New Chat
  - Ask simplechat.ai anything
---

## Learning Goals

By completing this challenge, you will:

- Build a simple AI chatbot.
- Work with a provided API to get responses for user questions.
- Create conversations and store them in local storage.
- Implement functionality to edit and delete conversations.
- Ensure the application is responsive on all devices.

## Requirements

You should create a web page that includes the following elements:

- Create an AI chatbot that matches the given layout.
- By default, users should see a small conversation between the user and the chatbot.
- Users can ask the following questions and get responses from the chatbot.
- Users can add new conversations. When a new conversation is added, its title should be the first question from the user.
- Conversations should be stored in local storage.
- Users can edit conversations' title.
- Users can delete conversations.
- The application should be responsive on all devices.
- Deploy the solution and submit Repository URL and Demo URL.

## Technical Details

To build the AI chatbot, you can use the [ChatGPT](https://openai.com/api/) or the [Hugging Face API](https://huggingface.co/). Please note that using the ChatGPT API may incur fees for accessing their services.

To display the default conversation and handle user interactions, you can use JavaScript and HTML.

For storing conversations, you can utilize the local storage feature of the browser.

For bonus points, you can make the application responsive using CSS media queries.

### Instructions for Building an AI Chatbot

#### 1. Set Up Your Project:

- Use Create React App to set up a new React project.

#### 2. Create the Chatbot Layout:

- Design the layout for the chatbot using React components and CSS.

#### 3. Fetch Data:

- Use JavaScript to fetch responses from the ChatGPT free version based on user questions.

#### 4. Display Default Conversation:

- Display a small conversation between the user and the chatbot by default.

#### 5. Add Conversations:

- Allow users to add new conversations. The title of a new conversation should be the first question from the user.

#### 5. Store Conversations:

- Store conversations in the local storage of the browser.

#### 6. Edit Conversations:

- Implement functionality to edit conversations' titles.

#### 7. Delete Conversations:

- Allow users to delete conversations.

#### 8. Deployment:

- Deploy your solution and provide the Repository URL and Demo URL for submission.

## Example Usage of ChatGPT and Hugging Face APIs

Here is a short example of how you can use the ChatGPT and Hugging Face APIs to build an AI chatbot:

1. Set up your project and install the necessary dependencies.

2. Import the required libraries and initialize the API credentials.

3. Create a function to send user questions to the API and receive responses.

```javascript
async function getChatbotResponse(question) {
  const response = await fetch(
    "https://api.openai.com/v1/engines/davinci-codex/completions",
    {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
        Authorization: "Bearer YOUR_API_KEY",
      },
      body: JSON.stringify({
        prompt: question,
        max_tokens: 50,
      }),
    }
  );

  const data = await response.json();
  return data.choices[0].text.trim();
}
```

4. Use the `getChatbotResponse` function to fetch responses from the ChatGPT API based on user questions.

```javascript
const userQuestion = "What is the weather like today?";
const chatbotResponse = await getChatbotResponse(userQuestion);
console.log(chatbotResponse);
```

5. Alternatively, you can use the Hugging Face API to get responses from models like GPT-3, GPT-2, or DialoGPT.

```javascript
async function getHuggingFaceResponse(question) {
  const response = await fetch(
    "https://api-inference.huggingface.co/models/DialoGPT/chat",
    {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
        Authorization: "Bearer YOUR_API_KEY",
      },
      body: JSON.stringify({
        messages: [
          { role: "system", content: "You are a helpful assistant." },
          { role: "user", content: question },
        ],
      }),
    }
  );

  const data = await response.json();
  return data.choices[0].message.content;
}
```

6. Use the `getHuggingFaceResponse` function to fetch responses from the Hugging Face API.

```javascript
const userQuestion = "What is the capital of France?";
const chatbotResponse = await getHuggingFaceResponse(userQuestion);
console.log(chatbotResponse);
```

**Remember to replace `YOUR_API_KEY` with your actual API key for both ChatGPT and Hugging Face APIs. Please note that you should never publicly share your API key as it can be used by others to access your account and potentially incur charges or misuse the API services.**

## Tech Stack

For this project, you can use HTML, CSS, and JavaScript. Consider using a frontend framework like React or Vue.js for additional functionality and ease of development. However, it is not required.

Good luck with the challenge!
