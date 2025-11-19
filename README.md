# 💰 Expense Tracker Automation — Telegram + Notion + AI

A fully automated expense tracking system built with n8n, Google Gemini AI, Telegram, and Notion.  
Simply send a message on Telegram like “Spent 45 on food 🍔”, and the bot will automatically record it in a Notion database with the correct category and value.

## 🧩 Technologies and Tools Used

- n8n (automation platform)
- Telegram Bot API
- Google Gemini Chat Model
- JavaScript (Code Node in n8n)
- Notion API

## ⚙️ Workflow Overview

Telegram → Gemini AI → JavaScript → Notion → Telegram Reply

Step-by-step logic:

1. Telegram Trigger  
Receives messages like: “Gastei 50 com transporte”.

2. AI Agent (Google Gemini)  
Extracts structured data such as:  
category: Transporte  
value: 50  
description: Uber

3. JavaScript Node  
Formats the data for Notion.

4. Notion Integration  
Creates a new record with:  
- Amount  
- Category  
- Date  
- Description  

5. Telegram Confirmation  
Sends back:  
“✅ Expense registered: 50 (Transporte)”

## 🖥️ Example Message Flow

User:  
Gastei 35 com comida  

Bot:  
✅ Expense registered: R$35 — Categoria: Comida 🍽️

## 📘 Example Notion Record

Date: 2025-11-19  
Description: Comida  
Category: Alimentação  
Amount: 35

## 🧠 Why This Project Matters

This automation simplifies daily expense tracking by combining:  
- Natural language input through Telegram  
- AI interpretation using Gemini  
- Structured, organized storage in Notion  

A practical example of using automation + AI to make personal finance effortless.

## 🛠️ Future Improvements

- Add monthly summaries with charts in Notion  
- Include automatic currency conversion  
- Add Google Sheets export for analytics  

📌 Developed as a personal automation project using n8n, Gemini, Telegram, and Notion.
