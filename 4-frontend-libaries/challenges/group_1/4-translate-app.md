---
title: "Translate App"
description: "As a Frontend developer, you will be given tasks to build an interactive application. In this challenge, you will build a simple translate application with a given API."
isNew: false
sort: 1
nature: "JavaScript"
skills:
  - "JavaScript"
  - "React"
  - "Reusable Components"
  - "Front-end libraries"
lessons:
  - 1-fundamentals/free-hosting-for-web-projects
userStories:
  - Create a translate application page that matches the given design.
  - By default, it should translate 'Hello, how are you' to French.
  - Users can change translating text with a maximum of 500 characters.
  - Users can see the translated text after selecting the Translate button. Optionally, users can see updates in real-time and you use debounce or throttling to optimize the application.
  - "Users can choose different languages to translate from. They should see at least 3 options: Detect Language, English and French."
  - Users can switch translation language and translated language.
  - Users can have the option to listen to the translating and translated texts.
  - Users can copy the translating and translated texts.
seo:
  title: "Translate App | Frontend, React project"
  description: "As a Frontend developer, you will be given tasks to build an interactive application. In this challenge, you will build a simple translate application with a given API. This project is great for working with Front-end libraries like React, Vue,..."
  keywords:
    - "translate app"
    - "frontend developer"
    - "interactive application"
challengeTexts:
  - Peace, nature, dream
  - Find and book a great experience.
---

## Learning Goals

By completing this challenge, you will:

- Build an interactive translate application.
- Implement translation functionality using a given API.
- Enhance your HTML, CSS, and JavaScript skills.
- Gain experience in creating real-time updates and optimizing the application.

## Requirements

You should create a web page that includes the following elements:

- Create a translate application page that matches the given design.
- By default, it should translate 'Hello, how are you' to French.
- Users can change translating text with a maximum of 500 characters.
- Users can see the translated text after selecting the Translate button. Optionally, users can see updates in real-time and you use debounce or throttling to optimize the application.
- Users can choose different languages to translate from. They should see at least 3 options: Detect Language, English and French.
- Users can switch translation language and translated language.
- Users can have the option to listen to the translating and translated texts.
- Users can copy the translating and translated texts.

## Technical Details

To fetch the data for the translation, you should make a POST request to the following URL:

```
https://mymemory.translated.net/doc/spec.php
```

Here's an example of how you can use the `fetch` API in JavaScript to retrieve the translation data from the provided URL:

```javascript
fetch("https://api.mymemory.translated.net/get", {
  method: "POST",
  body: JSON.stringify({
    q: "Hello, how are you",
    langpair: "en|fr",
  }),
  headers: {
    "Content-Type": "application/json",
  },
})
  .then((response) => response.json())
  .then((data) => {
    // Use the translated data here
  })
  .catch((error) => {
    // Handle any errors here
  });
```

### Instructions for Using a Frontend Library for Translate App Challenge

#### 1. Set Up Your Project:

- Use Create React App to set up a new React project.

#### 2. Create Components:

- Create a TranslateApp component to display the translate application page.
- Create a TranslateForm component to handle user input and translation requests.

#### 3. Fetch Data:

- Use the fetch API to retrieve translation data from the provided URL.

#### 4. Render Components:

- Use the TranslateApp component to render the translate application page.
- Use the TranslateForm component to handle user input and display the translated text.

#### 5. Real-time Updates:

- Implement real-time updates using debounce or throttling techniques.

#### 6. Language Options:

- Provide at least 3 language options: Detect Language, English, and French.

#### 7. Switch Languages:

- Allow users to switch between translation language and translated language.

#### 8. Text-to-Speech:

- Implement text-to-speech functionality for the translating and translated texts.

#### 9. Copy Text:

- Provide an option for users to copy the translating and translated texts.

#### Example Code

```js
// TranslateForm

import React, { useState } from "react";

function TranslateForm() {
  const [translatingText, setTranslatingText] = useState("Hello, how are you");
  const [translatedText, setTranslatedText] = useState("");

  const handleTranslate = () => {
    // Fetch translation data and set translatedText
  };

  return (
    <div className="translate-form">
      <textarea
        value={translatingText}
        onChange={(e) => setTranslatingText(e.target.value)}
        maxLength={500}
      />
      <button onClick={handleTranslate}>Translate</button>
      <div className="translated-text">{translatedText}</div>
    </div>
  );
}

export default TranslateForm;
```

## Tech Stack

For this project, you have the flexibility to use HTML, CSS, and JavaScript or a Front-end library like React, Vue, etc. Consider the learning curve and additional setup required when choosing a library.

Good luck with the challenge!
