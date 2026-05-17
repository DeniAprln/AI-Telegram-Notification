# AI-Telegram-Notification

# Google Sheets to Groq AI Telegram Automation

This automation monitors new form responses in Google Sheets, processes the data using Groq AI, and sends notifications to Telegram only for relevant entries.

## 🚀 Project Overview

This project creates an automated workflow that connects Google Sheets with Groq AI and Telegram. Every time a new entry is submitted via Google Form, the system analyzes the data using AI and sends a notification to Telegram if the entry is considered important.

## ✨ Key Features

- Real-time monitoring of new Google Sheets entries
- AI-powered filtering using Groq (`llama-3.1-8b-instant`)
- Sends Telegram notification only for relevant data
- Error handling with automatic retry
- Runs every 15 minutes

## 🛠️ Technologies Used

- Make.com (Automation Platform)
- Google Sheets
- Groq API
- Telegram Bot API

## 📊 Automation Flow

1. Google Sheets → Watch New Rows
2. HTTP Request → Groq AI (Chat Completions)
3. Filter → Continue only if AI returns "PROSES"
4. Telegram Bot → Send notification

## 📋 Files

- `GoogleSheets-Groq-Telegram.blueprint.json` → Make.com scenario blueprint
- `README.md` → Project documentation

## ⚠️ Setup Guide

1. Import the blueprint file into Make.com
2. Replace all placeholders:
   - `YOUR_GROQ_API_KEY_HERE`
   - `YOUR_SPREADSHEET_ID`
   - `YOUR_TELEGRAM_CHAT_ID`
3. Update Google Sheets and Telegram connections
4. Activate the scenario
