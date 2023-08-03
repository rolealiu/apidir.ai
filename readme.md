# APIDir.AI - Unlock AI Potential with Free API
## Free API Directory which is friendly to AI, with complete API documentation and easy for AI to understand and use.

[English](./readme.md) / [中文](./readme-chs.md) / [日本語](./readme-jp.md) 

[APIDir.AI](https://apidir.ai) is an innovative website dedicated to providing AI developers and tech enthusiasts with free APIs. We strive to offer a user-friendly interface that helps you easily find, use, and manage various APIs, unleashing the infinite potential of AI. Not only that, but we also label each API as "AI Friendly," making it easier for you to discover APIs that are comprehensible and seamlessly integrable into your projects.

🤖 95% of this project was developed, data collected, and analyzed by AI!

👍 Thanks to the outstanding developers who provided APIs to us!

## ⭐ Key Features

- **Free API Directory**: apidir.ai offers an extensive collection of free APIs covering a wide range of functionalities, enriching and diversifying your AI projects.
- **AI Friendly**: Each API is carefully labeled as "AI Friendly," ensuring that you can effortlessly find APIs that are easy to understand and integrate, thus boosting your development productivity.
- **Real-time Monitoring**: We continuously monitor the performance of each API, guaranteeing stability and reliability, so your projects can run smoothly without interruptions.

## 👍 Benefits of Using apidir.ai

- **Time-Saving**: With apidir.ai's intelligent search and AI-friendly labeling, you can quickly discover APIs suitable for your projects from a vast repository, saving precious time.
- **Lower Barriers**: We provide detailed API documentation and usage instructions, simplifying your learning curve and easing the integration process.


## 🚀 Quick Start

Website: 👉 [https://apidir.ai](https://apidir.ai) 👈

Explore API: 👉 [https://explore.apidir.ai](https://explore.apidir.ai) 

## 📚 API List

🦾 APIDir.AI provides free and unauthenticated APIs for easy integration with programs and AI, eliminating the need for third-party API authentication.

| API Name                  | Request Method | Path                  | Query Parameters                                      | Description                   |
|--------------------------|----------------|-----------------------|-------------------------------------------------------|-------------------------------|
| Search API          | GET     | https://get.apidir.ai   | id: API ID, used to precisely find a specific API </br></br> language: Language of API data </br></br> status: API running status </br></br> topics: API topics </br></br> price: API charging status </br></br> ai_friendly: AI-friendly for easier AI understanding and usage   | Get detailed information about an API, supports multiple parameters for filtering.</br></br>When passing the 'id', it will return a single API with detailed documentation (if available).             |
| Get API Topics       | GET     | https://topics.apidir.ai| -language   | Get API topics based on the specified language  |

## ⭐️ Python Code Example

```python
import requests

# Use the get.apidir.ai API to get detailed information about an API
def get_api_details(api_id):
    url = f'https://get.apidir.ai/?id={api_id}'
    response = requests.get(url)
    data = response.json()
    return data

# Example code - Get information about an API with ID 1
api_details = get_api_details('1')
print(api_details)

# Use the topics.apidir.ai API to get API topics for a specific language
def get_api_topics(language):
    url = f'https://topics.apidir.ai/?language={language}'
    response = requests.get(url)
    data = response.json()
    return data

# Example code - Get API topics for the English language
api_topics = get_api_topics('eng')
print(api_topics)
```

## ⭐️ JavaScript Code Example

```javascript
const fetch = require('node-fetch');

// Use the get.apidir.ai API to get detailed information about an API
async function getApiDetails(apiId) {
  const url = `https://get.apidir.ai/?id=${apiId}`;
  const response = await fetch(url);
  const data = await response.json();
  return data;
}

// Example code - Get information about an API with ID 1
getApiDetails('1')
  .then(apiDetails => console.log(apiDetails));

// Use the topics.apidir.ai API to get API topics for a specific language
async function getApiTopics(language) {
  const url = `https://topics.apidir.ai/?language=${language}`;
  const response = await fetch(url);
  const data = await response.json();
  return data;
}

// Example code - Get API topics for the English language
getApiTopics('eng')
  .then(apiTopics => console.log(apiTopics));
```


---

Thank you for using APIDir.AI. We look forward to seeing the amazing projects you create! 🚀
