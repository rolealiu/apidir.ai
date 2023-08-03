# APIDir.AI - 通过 API 解锁 AI 潜能
## 易于 AI（和开发者） 理解和使用的 API 目录。

[English](./readme.md) / [中文](./readme-chs.md) / [日本語](./readme-jp.md) 

[APIDir.AI](https://apidir.ai) 是一个创新的网站，专注于为AI开发者和科技爱好者提供免费API。我们致力于为您提供简单易用的界面，帮助您轻松查找、使用和管理各种API，释放无限的AI潜能。不仅如此，我们还为每个API添加了"AI友好"标签，帮助您快速发现易于理解和集成的API，提高开发效率。

🤖 本项目中有95%的部分由AI开发、数据收集和分析！

👍 感谢众多优秀开发者为我们提供API！

## ⭐ 主要特点

- **免费API目录**：apidir.ai提供丰富的免费API，涵盖广泛功能，丰富多样化您的AI项目。
- **AI友好**：每个API都经过精心标注为"AI友好"，确保您轻松找到易于理解和集成的API，提高开发效率。
- **实时监控**：我们持续监控每个API的性能，保证稳定性和可靠性，让您的项目无缝运行。

## 👍 使用APIDir.AI的好处

- **节省时间**：通过apidir.ai智能搜索和AI友好标签，您可以快速找到适合项目的API，节省宝贵时间。
- **降低门槛**：我们提供详细的API文档和使用说明，简化学习过程，轻松集成API。

## 🚀 快速入门

网站：👉 [https://apidir.ai](https://apidir.ai) 👈

探索API：👉 [https://explore.apidir.ai](https://explore.apidir.ai) 

## 📚 API列表

🦾 APIDir.AI提供免费的非认证API，便于与程序和AI轻松集成，无需第三方API认证。

| API名称            | 请求方法 | 路径                      | 查询参数                               | 描述                       |
|------------------|----------|-------------------------|---------------------------------------|--------------------------|
| 搜索API                | GET    | https://get.apidir.ai    | id：API ID，用于精确查找特定API </br></br> language：API数据语言 </br></br> status：API运行状态 </br></br> topics：API主题 </br></br> price：API收费状态 </br></br> ai_friendly：是否对AI友好，便于AI理解和使用   | 获取API的详细信息，支持多个参数进行过滤。</br></br>当传递'id'参数时，将返回带有详细文档（如果有）的单个API。 |
| 获取API主题        | GET    | https://topics.apidir.ai | -language                          | 获取指定语言的API主题         |

## ⭐️ Python代码示例

```python
import requests

# 使用get.apidir.ai API获取API的详细信息
def get_api_details(api_id):
    url = f'https://get.apidir.ai/?id={api_id}'
    response = requests.get(url)
    data = response.json()
    return data

# 示例代码 - 获取ID为1的API信息
api_details = get_api_details('1')
print(api_details)

# 使用topics.apidir.ai API获取特定语言的API主题
def get_api_topics(language):
    url = f'https://topics.apidir.ai/?language={language}'
    response = requests.get(url)
    data = response.json()
    return data

# 示例代码 - 获取英语语言的API主题
api_topics = get_api_topics('eng')
print(api_topics)
```

## ⭐️ JavaScript代码示例

```javascript
const fetch = require('node-fetch');

// 使用get.apidir.ai API获取API的详细信息
async function getApiDetails(apiId) {
  const url = `https://get.apidir.ai/?id=${apiId}`;
  const response = await fetch(url);
  const data = await response.json();
  return data;
}

// 示例代码 - 获取ID为1的API信息
getApiDetails('1')
  .then(apiDetails => console.log(apiDetails));

// 使用topics.apidir.ai API获取特定语言的API主题
async function getApiTopics(language) {
  const url = `https://topics.apidir.ai/?language=${language}`;
  const response = await fetch(url);
  const data = await response.json();
  return data;
}

// 示例代码 - 获取英语语言的API主题
getApiTopics('eng')
  .then(apiTopics => console.log(apiTopics));
```


---

感谢使用APIDir.AI，期待您创建出的精彩项目！🚀
```