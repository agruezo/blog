+++
date = "2025-04-16"
title = "AI Powered Dashboard"
author = "Alex"
hideComments=true
+++

# Building a Local AI-Powered KPI Dashboard with Streamlit and Ollama

In this project, I built a sleek, brand-aligned **business intelligence dashboard** powered entirely by **local AI** — no API keys, no cloud dependencies. Just **Python, Streamlit, and Ollama** running smart and fast right on my machine.

<!-- [{{< image src="/img/ai-powered-dashboard-thumb.png" alt="Data Science" position="center" style="border: 10px solid #23B0FF; padding: 8px; background: #1e202c;" >}}](/img/ai-powered-dashboard.png) -->

<a href="/img/ai-powered-dashboard-center-full.png" target="_blank" rel="noopener noreferrer">
  {{< figure src="/img/ai-powered-dashboard-center-thumb.png" alt="AI Powered Dashboard" position="center" style="border: 10px solid #23B0FF; padding: 8px; background: #1e202c;" caption="Click On Image" captionStyle="color: white;" >}}
</a>

---

## 🎯 The Goal

Create a lightweight yet powerful app that lets users:

- Upload or use built-in business KPI data
- Visualize revenue, profit, and conversion trends
- Generate AI-powered summaries and insights
- Ask follow-up questions using natural language
- Export clean PDF reports — charts included

---

## 🔧 The Tech Stack

| Layer         | Tech                      |
|---------------|---------------------------|
| Frontend      | Streamlit (Python)        |
| Charts        | Matplotlib                |
| AI Engine     | Ollama + Mistral model    |
| PDF Export    | FPDF                      |
| Storage       | `tempfile`, CSV, session  |

---

## 🧱 What the App Does

#### 📊 1. Upload or Simulate Business Data

The app loads default revenue, expenses, leads, and client data — or allows the user to upload a custom CSV. It auto-generates calculated fields like:

- **Profit** = Revenue - Expenses  
- **Conversion Rate** = Clients ÷ Leads

---

#### 📈 2. Visualize KPIs

Three clean, responsive charts are generated with Matplotlib:

- Revenue vs. Expenses (Line Chart)
- Monthly Profit (Bar Chart)
- Conversion Rate (Line Chart)

---

#### 🧠 3. Generate AI Summaries

Click a button and get a GPT-style summary of your data using **Ollama** + a locally-running **Mistral** model — no API required.

Summaries are cached in `session_state`, so they persist between interactions and don't get overwritten by the chat module.

---

#### 💬 4. Ask the Model Business Questions

Type in a natural language question like:

> “What’s the trend in profit over the past 3 months?”

The app feeds both the KPI data and the question to Ollama and returns a contextual, AI-generated answer.

---

#### 📄 5. Export PDF Reports

Generate branded PDF reports including:

- Title and summary section
- Embedded KPI charts
- Styled with your brand colors

---

#### 📥 6. Download Raw Data

Export your data as a CSV at any time.

---

## 🧠 Why It’s Cool

- **Offline AI**: Runs entirely on your machine with Ollama (tested with Mistral, Gemma, and Phi)
- **Customizable**: Plug in any dataset or model
- **Scalable**: Easy to repurpose for client reporting, SaaS, or internal BI tooling
- **Free and Private**: No API usage, no cloud costs, no data leaving your machine

---

## 🚀 Next Steps

I’ll continue refining it by:

- Adding markdown rendering in PDFs
- Supporting advanced formatting (headings, lists)
- Packaging it for internal use or monetization

Stay tuned — or <a href="https://www.gruezo.com/resume#contact" target="_blank" rel="noopener noreferrer">reach out</a> if you want help building something like this for your team.

---