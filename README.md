# 🤖 AI CRM Assistant

An AI-powered CRM automation workflow built with **n8n**, **Ollama**, **JavaScript**, **Gmail API**, and **Google Sheets**. The workflow automatically extracts lead information from user input, validates the data, calculates a lead score based on business rules, sends email notifications for high-priority leads, and stores all leads in a CRM database.

---

## 🚀 Features

- 🤖 AI-powered Lead Information Extraction
- 📋 Structured JSON Output
- 🧠 Business Rule-based Lead Scoring Engine
- 🔥 Automatic Hot / Warm / Cold Lead Classification
- ✅ Lead Validation
- 📧 Automatic Email Alert for Hot Leads
- 📊 Google Sheets CRM Integration
- 🔄 Duplicate Lead Update
- ❌ Invalid Lead Detection & Logging
- 🕒 Automatic Timestamp
- 🎨 Professional HTML Email Template
- ⚡ End-to-End Workflow Automation

---

## 🛠️ Tech Stack

- **n8n**
- **Ollama**
- **JavaScript**
- **Google Sheets API**
- **Gmail API**
- **JSON**
- **AI Agent**

---

## 📌 Workflow Overview

```text
Chat Trigger
      │
      ▼
AI Lead Extractor
      │
      ▼
Lead Scoring Engine
      │
      ▼
Lead Validation
      │
 ┌────┴─────┐
 │          │
False      True
 │          │
 ▼          ▼
Invalid   Hot Lead Check
 Leads        │
              ▼
      Send Gmail Alert
              │
              ▼
      Google Sheets CRM
```

---

## 📊 Lead Scoring Logic

The lead score is calculated using configurable business rules.

| Criteria | Score |
|----------|------:|
| Decision Maker (CEO/CTO/Founder/Owner) | +30 |
| Budget ≥ 20,000 | +30 |
| Budget ≥ 10,000 | +20 |
| Budget ≥ 5,000 | +10 |
| High Urgency | +20 |
| Medium Urgency | +10 |
| Company Provided | +10 |
| Valid Email | +10 |

### Lead Classification

- 🔥 **Hot** → Score ≥ 80
- 🟡 **Warm** → Score ≥ 50
- ⚪ **Cold** → Score < 50

---

## 📧 Automated Actions

### Hot Lead

- Send Professional HTML Email
- Save/Update Google Sheets CRM

### Warm Lead

- Save to Google Sheets

### Cold Lead

- Save to Google Sheets

### Invalid Lead

- Save to Invalid Leads Sheet
- Store Validation Errors

---

## 📂 Project Structure

```
AI-CRM-Assistant/
│
├── workflow/
│   └── AI_CRM_Assistant_v1.0.json
│
├── screenshots/
│   ├── workflow.png
│   ├── gmail-alert.png
│   ├── google-sheet.png
│   └── chat-test.png
│
├── README.md
└── LICENSE
```

---

## 📸 Screenshots

### Workflow

> Add screenshot here

### Gmail Notification

> Add screenshot here

### Google Sheets CRM

> Add screenshot here

---

## 💡 Future Improvements

- Slack Notifications
- Microsoft Teams Integration
- CRM API Integration
- Lead Assignment
- AI Follow-up Email
- Dashboard & Analytics
- Multi-Agent AI Workflow

---

## 🎯 Use Cases

- Sales Automation
- Lead Qualification
- CRM Automation
- AI Sales Assistant
- Marketing Automation
- Customer Acquisition

---

## 👨‍💻 Author

**Sajib Hasan**

GitHub: https://github.com/sajibhasan

---

## ⭐ If you found this project useful, please consider giving it a Star.