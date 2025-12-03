## 🚀 n8n Workflows for Insider AI Weekend

This repository contains **n8n workflows** created during the **Insider AI Weekend** event, leveraging AI for various automation and content generation tasks.

These workflows utilize the **Google Gemini Chat Model** for Natural Language Processing (NLP) and content creation, integrating its capabilities with services like Slack, Google Sheets, Gmail, and external APIs via HTTP requests. The core goal of these examples is to demonstrate how to build **smart automation agents** that can interact with real-world data sources (like weather and stock market APIs) and execute complex, personalized communication tasks without manual intervention.

---

### 📂 Workflows Overview

| File Name | Purpose | Key Technologies & Integrations |
| :--- | :--- | :--- |
| `stock-weather-news-briefing.json` | Creates a **personalized daily briefing** for a specified user. It gathers **weather data**, **Apple (AAPL) stock data**, and **news**, then uses an AI Agent to compile it into a friendly, conversational messages, which is sent via Slack. | **HTTP Request** (OpenWeatherMap, Finnhub), **Google Gemini Chat Model** (AI Agent), **Slack**. |
| `message_summarizer_slack.json` | Retrieves messages from a specified Slack channel, uses the **Google Gemini Chat Model** to create a **concise, 50-word summary** of the discussions grouped by author, and posts the summary back to Slack. | **Slack** (Message Search, Send Message), **Google Gemini Chat Model** (AI Agent). |
| `sheet-email-automation.json` | Reads rows from a **Google Sheets** document (containing Name, Email, Business Type) and uses the **Google Gemini Chat Model** to generate a **personalized, professional outreach email** introducing a logistics application, which is then sent via Gmail. | **Google Sheets** (Read Data), **Google Gemini Chat Model** (AI Agent), **Gmail** (Send Email). |

---

These examples serve as a practical starting point for anyone looking to integrate large language models (LLMs) into their business processes using n8n. By showcasing different data sources—from structured tables in Google Sheets to real-time API responses—and various output channels like Slack and Gmail, the workflows illustrate the versatility of n8n's visual programming and the power of the Google Gemini API to handle dynamic content generation, summarization, and personalization at scale.
