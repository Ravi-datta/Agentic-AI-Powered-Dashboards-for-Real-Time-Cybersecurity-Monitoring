
# Agentic AI for Dynamic Dashboards and Real-Time Cybersecurity Insights

![Project Status](https://img.shields.io/badge/status-Completed-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Made with React](https://img.shields.io/badge/frontend-React-lightblue)
![SecureGPT](https://img.shields.io/badge/AI-SecureGPT-critical)

## 🧠 Overview

In today’s fast-paced digital landscape, organizations face immense challenges in monitoring and maintaining cybersecurity across diverse data sources. This project presents an **AI-powered, real-time dashboard system** that processes natural language prompts to generate dynamic cybersecurity insights tailored to both technical and non-technical users.

Leveraging **SecureGPT**, AWS Lambda, and Plotly visualizations, the system fetches, analyzes, and visualizes security data from logs, alerts, and task datasets, empowering stakeholders with instant, actionable intelligence — **no manual scripting or data wrangling required**.

## 📌 Problem Statement

Organizations often struggle to unify and interpret complex security data from diverse sources — such as anomaly logs, network events, and compliance alerts. Static dashboards fall short in delivering real-time, role-specific insights, leading to delayed responses, compliance violations, and increased risk exposure.

This project aims to solve that with:
- A **multi-agent AI system** that interprets user queries.
- **Real-time dashboards** tailored to stakeholder roles.
- **Dynamic visualizations** that eliminate manual effort.

## 🛠 Features

- 🔍 **Natural Language Query Support** (via SecureGPT)
- 📊 **Role-Based Dashboards** (for CISOs, compliance officers, engineers)
- 📈 **Interactive Charts** (line, bar, pie, heatmaps)
- 🧠 **Auto-Summarized Insights** (executive-level summaries)
- 🔐 **Secure Cloud Architecture** (AWS S3, Lambda, API Gateway)
- ⚙️ **Serverless Deployment** for scalable performance

## 🧰 Tech Stack

| Component              | Technology Used           |
|------------------------|---------------------------|
| Frontend               | React (Create React App)  |
| Backend                | AWS Lambda                |
| AI Integration         | SecureGPT (via API)       |
| Visualizations         | Plotly                    |
| Storage                | Amazon S3                 |
| CI/CD & Testing        | Postman, React Testing    |
| Security               | API Gateway, API Keys     |

## 📐 Architecture Diagram

![System Architecture](architecture_diagram.png)

## 📂 Project Structure

```
Daen-690-Project/
├── SecureGPT agent.py             # SecureGPT interface for prompt interpretation
├── Dashboard rendering agent.py   # Chart rendering via Plotly
├── Pipeline agent.py              # Orchestrates flow between agents
├── Summary agent.py               # Executive-level narrative generation
├── Validation agent.mjs           # API key and input validation
├── User Interface/                # React-based UI
│   ├── public/                    # HTML and manifest
│   └── src/                       # Components, assets, logic
```

## ⚙️ Installation & Setup

### Backend (AWS Lambda)
1. Create required Lambda functions (`SecureGPT`, `DashboardRenderer`, `SummaryAgent`, etc.)
2. Configure S3 buckets for input and output datasets.
3. Set environment variables and deploy using AWS CLI or Console.

### Frontend (React App)
```bash
cd User\ Interface
npm install
npm start
```
- Open `http://localhost:3000` to interact with the app.

## 📊 How to Use

1. Open the dashboard interface.
2. Enter a **natural language prompt**, e.g., “Show anomaly trends for the last 30 days.”
3. The system:
   - Sends query to SecureGPT
   - Selects datasets
   - Renders charts
   - Generates narrative summary
4. View and download the dashboard.

## 📈 Example Use Case

- **Prompt**: "Summarize this month’s top 3 cybersecurity threats"
- **Output**:
  - Executive Summary
  - Line chart of threat frequency
  - Risk heatmap
  - Compliance status table

## 🧪 Testing & Performance

- 📉 Load tested with **up to 4 million rows**
- ⏱ Avg. dashboard generation time: **<10 seconds**
- ✅ 92% accuracy in chart relevancy
- 📊 Precision: 92.72%, Recall: 84.53%, F1: 88.40%

## 🚀 Future Enhancements

- 🤖 Voice-based prompt support
- 🔁 Cross-dataset correlation
- 🌐 Mobile app support
- 📢 SMS/Email alerts for high-risk events
- 🧬 3D & AR-based visualizations

## 👨‍💻 Team

- Ravi Datta Rachuri  
- Shuchi Nirav Shah  
- Akash Bejugam  
- Datha Vaishnavi Kondur  
- Yashaswi Gurram  
- Vardhan Tharlapally

