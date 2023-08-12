# Article Summarizer

## Live Link / Demo Link: 🔗
[Deployed app](https://article-summarizer-ai.vercel.app/)

## About the Project: 📚
This project aims to develop an Article Summarizer application leveraging ReactJS and 
Vite as the front-end technologies, along with the integration of RapidAPI for accessing 
news and article content. The application provides users with the ability to summarize 
various news articles, enhancing the reading experience by condensing lengthy content into concise summaries.

## Screenshots: 📷
<img src="https://github.com/alibinauanov/article-summarizer-ai/blob/main/sumz.gif" width="400" height="400">

## Technologies Used: ☕️ 🐍 ⚛️
* React.js
* JavaScript
* Redux
* SCSS
* API

## Setup / Installation: 💻
#### Install all dependecies
```npm i```

#### Run Project
```npm run dev```

#### API
Open this [link](https://rapidapi.com/restyler/api/article-extractor-and-summarizer) and have your own API KEY.</br>

## Approach: 🚶
#### article.js
In this file, the article API is created using the createApi function from @reduxjs/toolkit/query/react. 
The RapidAPI key is retrieved from the environment variables, and the base query is configured to make 
requests to the article extraction and summarization API. The endpoint is defined to retrieve article 
summaries by providing the article URL and desired summary length.

#### demo.jsx
This file represents the core functionality of the Article Summarizer application. It uses React state 
to manage article data, including the article URL and its summary. The application supports fetching 
summaries through a lazy query provided by Redux Toolkit's API, which communicates with the article API. 
Users can submit article URLs, and the application fetches and displays the summaries. It also allows users 
to copy article URLs for easy sharing and maintains a browsing history of articles for quick access.

#### hero.jsx
The Hero component represents the header section of the application. It showcases the project's logo 
and provides a link to the project's GitHub repository. The header also includes a title and description 
that highlight the application's purpose of simplifying article reading using the power of OpenAI's GPT-4 model.
