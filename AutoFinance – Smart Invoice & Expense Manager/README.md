# 📊 AutoFinance – Smart Invoice & Expense Manager

**AutoFinance** is a smart finance automation system built using **n8n** and **Google Gemini AI**.
It streamlines invoice processing, expense tracking, and financial reporting by automatically extracting, organizing, and analyzing financial data from emails — turning scattered information into structured insights.

---

## 📘 Overview

Manual finance management often leads to missed details, errors, and wasted time.
AutoFinance solves this by automating the **end-to-end workflow** of collecting invoices, parsing payment information, updating Google Sheets, and generating AI-based financial summaries.
This project demonstrates how **automation + AI** can simplify real-world business operations efficiently.

---

## ✨ Key Features

* **Automated Email Monitoring:** Detects new invoice or expense emails in real time.
* **Smart Data Extraction:** Parses key details such as invoice ID, client name, amount, date, and payment status.
* **Centralized Record Management:** Automatically logs data in Google Sheets for ongoing tracking.
* **AI-Driven Financial Insights:** Uses **Gemini AI** to summarize income, expenses, and profit trends.
* **Automated Monthly Reports:** Generates clear, formatted summaries and sends them via Gmail.
* **Completely Hands-Free:** Once deployed, the system runs continuously without manual effort.

---

## 🧩 Workflow Components

| Component                | Function                                                 |
| ------------------------ | -------------------------------------------------------- |
| **Gmail Trigger**        | Monitors inbox for incoming invoices or expense reports. |
| **AI Parsing (Gemini)**  | Extracts structured financial data from email body text. |
| **Google Sheets Node**   | Logs all transactions into a structured spreadsheet.     |
| **Data Filter Function** | Separates income from expenses for clarity.              |
| **AI Summary Node**      | Generates monthly reports summarizing totals and trends. |
| **Gmail Send Node**      | Emails formatted financial reports automatically.        |


<img width="1084" height="468" alt="workflow" src="https://github.com/user-attachments/assets/869983ad-4fb8-4fff-9c90-e71cc2497a88" />

---

## 🧠 Technical Stack

* **Platform:** n8n (Visual Workflow Automation)
* **AI Model:** Google Gemini AI (for NLP & summarization)
* **Data Storage:** Google Sheets
* **Communication:** Gmail API
* **Logic Layer:** Custom JavaScript & JSON processing

---

## 🔄 Workflow Process

1. **Trigger:** A new invoice or payment email arrives in Gmail.
2. **Extraction:** Gemini AI processes and extracts financial fields.
3. **Logging:** n8n appends the extracted data to a Google Sheet.
4. **Analysis:** AI summarizes the month’s financial performance.
5. **Reporting:** The summary is formatted and emailed to the user.

---

## 💡 Benefits

* Saves hours of manual bookkeeping
* Ensures accuracy in financial reporting
* Provides AI-generated insights instantly
* Integrates seamlessly with existing Google tools

---

**Areeba Bushra**
*Data Science & AI Enthusiast | Automation Developer*
📍 Based in Pakistan


