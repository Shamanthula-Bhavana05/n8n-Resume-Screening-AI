# n8n-Resume-Screening-AI

# 🤖 AI HR Automation System – Resume ATS Checking + Auto Shortlisting

This project automates the entire **resume screening process** using n8n, Python, and AI models.  
It extracts candidate data from uploaded resumes, calculates ATS score, stores data into Google Sheets,  
and sends **automated emails** for shortlisted candidates.

---

## 🖥 Demo Video
📺 YouTube Link: *https://youtu.be/Sfb0qjQiB7I*

---

## 📸 Workflow Snapshot

> Full Automation Flow in n8n

<img width="1920" height="859" alt="Resume ATS Friendly-Append to Sheets and Sending Mails" src="https://github.com/user-attachments/assets/dc798441-38da-4e3b-9858-81899e0d6495" />

---

## ✨ Features
- 📄 Resume Extraction from PDF  
- 🎯 ATS Score Calculation using AI  
- 📊 Data Append/Update in Google Sheets  
- ✉️ Auto Email Replies to Selected Candidates  
- 🧠 N8N-based scalable automation  
- 🔍 Filtering logic for shortlist criteria  

---

## 🔧 Tech Stack & Services
| Component | Technology |
|----------|------------|
| Automation | n8n |
| AI Model | Gemini / ChatGPT / LLM |
| Scripting | Python |
| Storage | Google Sheets |
| Communication | Gmail API |
| Messaging | Telegram Trigger |

---

## 🏗 Architecture Overview
```mermaid
flowchart LR
A[Upload Resume via Telegram] --> B[Extract Text from PDF]
B --> C[AI Model: ATS Score & Parsing]
C --> D[Google Sheets: Store Data]
C --> E{Shortlist Rule?}
E -->|Yes| F[Send Shortlisted Email]
E -->|No| G[Send Rejection/Thank You Message]
