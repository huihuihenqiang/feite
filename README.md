# Fit Fitness Platform 💪

# 【更新】2024.10.8新加入板块：
![图片](https://github.com/user-attachments/assets/ab61b2c5-af2d-4d66-8dcc-a869e0a0df01)

## 爬虫板块介绍
通过自动化方式从网络上抓取特定健身知识数据。使用了 Python 的 `requests` 和 `BeautifulSoup` 等库实现网页的请求与解析。支持多种数据格式输出，并具有错误处理与代理切换功能。

### 主要功能
- **数据抓取**：通过自定义 URL 抓取网页内容，支持动态与静态页面。
- **数据解析**：使用 `BeautifulSoup` 解析 HTML，提取目标数据。
- **存储与输出**：抓取的数据可以输出为 JSON、CSV 等格式，支持文件存储或数据库插入。
- **错误处理**：处理网络请求中的常见错误，如 404、超时等。
- **代理与延迟**：支持通过代理进行爬取，避免 IP 被封禁，并设置请求延迟模拟人工访问。

### 未来工作
- 增加对 JavaScript 动态加载页面的处理。
- 实现分布式爬虫，提高爬取效率。
## Web Scraping Section 
The web scraping module in this project automates the process of extracting specific exercise data from websites. It uses Python's `requests` and `BeautifulSoup` libraries for making HTTP requests and parsing HTML content. The module supports various output formats and includes error handling and proxy switching.

### Key Features
- **Data Scraping**: Fetch content from webpages via custom URLs, supports both static and dynamic pages.
- **Data Parsing**: Use `BeautifulSoup` to parse HTML and extract target data.
- **Storage & Output**: Data can be saved in JSON, CSV, and other formats, supporting file storage or database insertion.
- **Error Handling**: Handles common network issues such as 404 errors, timeouts, etc.
- **Proxy & Delay**: Supports proxy scraping to prevent IP blocking and allows setting request delays to simulate human behavior.

### Future Work
- Add support for handling JavaScript dynamically-loaded pages.
- Implement distributed scraping for improved efficiency.
![图片](https://github.com/user-attachments/assets/3bb73c99-c90d-48c8-bad0-406ce7c1b2a7)

## 智能健身对话系统 
本项目的智能健身对话系统使用人工智能技术，为用户提供个性化的健身指导与互动。该系统通过调用大模型（通义千问）生成自然语言对话，帮助用户规划健身计划、解答健身问题，甚至提供实时健身建议。

### 主要功能
- **个性化健身对话**：基于用户输入，通过 AI 生成针对性建议，包括训练计划、饮食推荐和动作指导。
- **自然语言处理**：通过 GPT 大模型，能够理解用户需求，进行流畅的对话。
- **实时反馈**：用户可以通过对话获得即时的健身建议和反馈，提升运动体验。
- **多轮对话**：支持复杂的多轮对话，帮助用户进行长时间的健身规划和跟踪。

## Intelligent Fitness Dialogue System (English)
This project’s Intelligent Fitness Dialogue System leverages AI technologies to offer personalized fitness guidance and interactive conversations. By utilizing large language models (such as the qwen series), the system generates natural language dialogues to help users plan workouts, answer fitness-related questions, and even provide real-time fitness advice.

### Key Features
- **Personalized Fitness Dialogue**: Based on user input, the AI generates tailored advice, including workout plans, dietary recommendations, and exercise instructions.
- **Natural Language Processing**: Uses GPT models to understand user needs and conduct smooth conversations.
- **Real-time Feedback**: Users receive instant fitness advice and feedback to enhance their workout experience.
- **Multi-turn Conversations**: Supports complex multi-turn dialogues for long-term fitness planning and progress tracking.


## Overview

Welcome to the Fit Fitness Platform! This platform is designed to offer a comprehensive fitness experience through both online and offline services. Below, we will introduce the online components of our platform, including the technical details and programming techniques used to implement various features.

![首页页面](https://user-images.githubusercontent.com/99072450/233411174-37cace23-2c6e-4710-9f91-4a448762c347.png)

## Online Features

### 1. Dashboard 📊
- **Statistics Display 📈**
  - **Implementation:** Utilizes data visualization libraries such as ECharts to present workout statistics and progress in an engaging manner.
  - **Technical Detail:** Data is fetched from the backend cloud database using WeChat Mini Program cloud functions and displayed using ECharts components.

![设置运动页面](https://user-images.githubusercontent.com/99072450/233411528-59ffc671-a113-4632-8dfa-33be49ea81c8.png)
![预约入口页面](https://user-images.githubusercontent.com/99072450/233411555-3442d13c-705b-4102-ad34-d1c061033a54.png)

- **Personalized Training Courses 🏋️**
  - **Implementation:** Offers tailored workout plans by integrating with machine learning algorithms hosted on cloud services.
  - **Technical Detail:** User data and preferences are analyzed using TensorFlow.js to generate personalized training plans.

### 2. Live Classes 📹
- **Real-time Interaction 🤝**
  - **Implementation:** Uses WebSocket connections to provide real-time video streaming and interaction capabilities.
  - **Technical Detail:** WebSocket API ensures low-latency communication between the client and the server, facilitating seamless live class experiences.

- **Class Replay 🔄**
  - **Implementation:** Records live sessions and stores them in cloud storage for on-demand access.
  - **Technical Detail:** Cloud storage solutions like WeChat Cloud Storage are utilized to manage and serve replay videos efficiently.

### 3. Community 🌐
- **Activity Sharing 📢**
  - **Implementation:** Similar to social media, users can post updates, share achievements, and interact with others.
  - **Technical Detail:** Implements a news feed using a combination of cloud database queries and real-time updates with WebSocket.

- **Feedback and Comments 💬**
  - **Implementation:** Allows users to provide feedback and comment on posts using a structured comment system.
  - **Technical Detail:** Utilizes cloud database capabilities to handle CRUD operations for comments and feedback.
  - 
![健身圈页面](https://user-images.githubusercontent.com/99072450/233411698-ed734254-5fa7-4d01-888b-8d156d165b82.png)
![管理员审核页面](https://user-images.githubusercontent.com/99072450/233411740-9e5d6800-a3c5-4bd8-8d9d-3b0bec65c1cd.png)
### 4. Events 🎉
- **Public Events 🏆**
  - **Implementation:** Hosts various fitness events, which users can join and participate in through the platform.
  - **Technical Detail:** Event details are managed through cloud database entries, and user participation is tracked using unique identifiers.

- **Competitions and Challenges 🥇**
  - **Implementation:** Organizes fitness competitions and challenges to engage users and offer rewards.
  - **Technical Detail:** Gamification elements are added using cloud functions to manage competition data and user progress.

## Additional Features

### 1. Word Search 
- **Implementation:** Provides a search functionality to quickly find specific words or terms within the app.
  - **Technical Detail:** Uses a search index built with cloud database full-text search capabilities for efficient querying.
  - 
![百宝箱页面](https://user-images.githubusercontent.com/99072450/233411471-8f3e224c-baa0-4d91-9a0d-0d541f0453c2.png)
![搜索结果页面](https://user-images.githubusercontent.com/99072450/233411648-04da85eb-870c-4c99-b31e-1247c8842116.png)
### 2. Registration 
- **Implementation:** Simple and secure user registration system.
  - **Technical Detail:** Implements WeChat Mini Program's built-in authentication services combined with cloud database for user data storage.
  - 
![注册页面](https://user-images.githubusercontent.com/99072450/233411599-516b7bb8-fc78-40af-aa4a-341eb73a6a65.png)

### 3. Pomodoro Timer 
- **Implementation:** Includes a Pomodoro timer to help users manage their workout and rest periods effectively.
  - **Technical Detail:** Timer functionality is built using JavaScript and managed state within the Mini Program framework.
  - 
![番茄时钟页面](https://user-images.githubusercontent.com/99072450/233411498-7e6bc45b-69fd-406f-97d2-c325d904dfd1.png)

## Technical Stack

- **WeChat Mini Program Development Platform**
- **WeChat Cloud Services **
- **JavaScript**
- **ECharts for Data Visualization**
- **TensorFlow.js for Machine Learning**
- **WebSocket for Real-time Communication**

## Getting Started 🚀

1. **Sign Up 📝**
   - Create an account to access all online features. Join us and start your fitness journey today!

2. **Browse Courses 🔍**
   - Explore various live and recorded fitness classes. Find the perfect workout that fits your needs.

3. **Join the Community 🤗**
   - Connect with other fitness enthusiasts. Share your journey and grow together.

4. **Track Your Progress 📅**
   - Monitor your workout statistics and achievements. Stay on top of your goals and celebrate your progress.

## Contact Us 📧

For any inquiries or support, feel free to contact us at [1870586279@qq.com].

---

# 菲特健身平台 💪

## 概述

欢迎来到菲特健身平台！本平台旨在通过线上和线下服务提供全面的健身体验。下面我们将介绍平台的线上部分，包括技术细节和实现各种功能的编程技巧。

## 线上功能

### 1. 仪表盘 📊
- **统计数据展示 📈**
  - **实现：** 利用ECharts等数据可视化库以引人入胜的方式展示锻炼统计数据和进度。
  - **技术细节：** 使用微信小程序云函数从后端云数据库获取数据，并使用ECharts组件进行展示。

- **个性化训练课程 🏋️**
  - **实现：** 通过集成云服务上托管的机器学习算法提供定制化的锻炼计划。
  - **技术细节：** 使用TensorFlow.js分析用户数据和偏好，生成个性化的训练计划。

### 2. 直播课程 📹
- **实时互动 🤝**
  - **实现：** 使用WebSocket连接提供实时视频流和互动功能。
  - **技术细节：** WebSocket API确保客户端和服务器之间的低延迟通信，促进无缝的直播课程体验。

- **课程重播 🔄**
  - **实现：** 录制直播课程并存储在云存储中，供按需访问。
  - **技术细节：** 使用微信云存储解决方案有效管理和提供重播视频。

### 3. 社区 🌐
- **活动分享 📢**
  - **实现：** 类似于社交媒体，用户可以发布更新、分享成就并与他人互动。
  - **技术细节：** 使用云数据库查询和实时更新功能实现动态消息流。

- **反馈与评论 💬**
  - **实现：** 允许用户提供反馈并对帖子进行评论，使用结构化评论系统。
  - **技术细节：** 利用云数据库功能处理评论和反馈的增删改查操作。

### 4. 活动 🎉
- **公共活动 🏆**
  - **实现：** 举办各种健身活动，用户可以通过平台加入并参与。
  - **技术细节：** 通过云数据库条目管理活动详情，并使用唯一标识符跟踪用户参与情况。

- **竞赛和挑战 🥇**
  - **实现：** 组织健身竞赛和挑战以吸引用户并提供奖励。
  - **技术细节：** 使用云函数添加游戏化元素，管理竞赛数据和用户进度。

## 附加功能

### 1. 词语搜索
- **实现：** 提供搜索功能，快速找到应用内的特定词语或术语。
  - **技术细节：** 使用云数据库全文搜索功能构建的搜索索引，以实现高效查询。

### 2. 注册
- **实现：** 简单且安全的用户注册系统。
  - **技术细节：** 结合微信小程序内置的认证服务和云数据库进行用户数据存储。

### 3. 番茄钟
- **实现：** 包含一个番茄钟，帮助用户有效管理锻炼和休息时间。
  - **技术细节：** 使用JavaScript和小程序框架内的状态管理功能构建计时器功能。

## 技术栈

- **微信小程序开发平台**
- **微信云服务（云开发）**
- **JavaScript**
- **ECharts 数据可视化**
- **TensorFlow.js 机器学习**
- **WebSocket 实时通信**

## 快速开始 🚀

1. **注册 📝**
   - 创建账户以访问所有线上功能。加入我们，开启您的健身之旅吧！

2. **浏览课程 🔍**
   - 探索各种直播和录制的健身课程。找到适合您的完美锻炼课程。

3. **加入社区 🤗**
   - 与其他健身爱好者连接。分享您的旅程，一起成长。

4. **跟踪进度 📅**
   - 监控您的锻炼统计数据和成就。紧跟您的目标，庆祝您的进步。

## 联系我们 📧

如有任何疑问或需要支持，请随时联系我们：[1870586279@qq.com]。

结构：
![默认状态-1x](https://user-images.githubusercontent.com/99072450/233412158-18408574-7c40-4a00-99c5-73c1066beb11.png)

如果想要部署和尝试的可以联系我，后期也会不断更新。因为使用了云开发，新手部署起来还是有一些难度的。
![图片](https://user-images.githubusercontent.com/99072450/233413000-cb71be5d-3ab3-4168-91d0-53a1406d3b86.png)



























