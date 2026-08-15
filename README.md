# 📧 Daily Motivational Quote Email Automation

An automated email workflow built with **n8n** that fetches a daily motivational quote from the **ZenQuotes API** and sends it to a configured Gmail account every morning.

## 🚀 Project Overview

This project automates the process of receiving a motivational quote every morning.

The workflow runs automatically at **7:35 AM**, retrieves the day's quote through the ZenQuotes API, and sends a formatted email containing the quote and its author. The workflow successfully sends the email through Gmail.

## 🔄 Workflow

```text
Schedule Trigger
      ↓
Fetch Daily Quote
      ↓
Send Morning Email
      ↓
     Gmail
```

### Workflow Steps

1. **Schedule Trigger**

   * Runs automatically every morning at **7:35 AM**.
   * Uses the n8n Schedule Trigger node.

2. **Fetch Daily Quote**

   * Sends a request to the ZenQuotes API.
   * Retrieves the daily quote and author information.

3. **Send Morning Email**

   * Sends an HTML-formatted email through Gmail.
   * The email contains the motivational quote, author, and current date.

## ✨ Features

* ⏰ Automated daily scheduling
* 🌐 API integration with ZenQuotes
* 📧 Automated Gmail delivery
* 💬 Dynamically generated motivational content
* 📅 Automatically generated email date
* 🔄 Fully automated workflow with no manual intervention

## 🛠️ Technologies Used

* **n8n** — Workflow automation
* **ZenQuotes API** — Daily quote source
* **Gmail** — Email delivery
* **REST API** — Data retrieval
* **JSON** — Workflow configuration

## 📂 Repository Structure

```text
daily-motivational-quote-email-n8n/
│
├── daily_motivational_quote_email.json
└── README.md
```

## ⚙️ How to Use

### 1. Install or access n8n

Create an n8n account or use an existing n8n instance.

### 2. Import the workflow

1. Open n8n.
2. Select **Import from File**.
3. Choose:

```text
daily_motivational_quote_email.json
```

4. Import the workflow.

### 3. Configure Gmail

Connect your Gmail account to the **Send Morning Email** node.

Set the recipient email address to the address where you want to receive the daily quote.

### 4. Activate the workflow

After configuring Gmail:

1. Test the workflow manually.
2. Confirm that the email is received.
3. Activate the workflow.

The workflow will then execute according to the configured schedule.

## 📧 Example Email

**Subject:**

```text
Your Daily Motivation - August 15, 2026
```

**Email:**

> Good morning!

> "Your daily motivational quote"

> — Author

The workflow uses dynamic expressions to insert the quote, author, and current date into the email.

## 🔐 Security

This repository does **not** contain Gmail passwords, OAuth access tokens, or other authentication secrets.

Before importing and using the workflow, configure your own Gmail credentials in n8n.

**Never commit API keys, passwords, OAuth tokens, or private credentials to GitHub.**

## 🎯 Learning Outcomes

This project demonstrates practical experience with:

* Workflow automation
* API integration
* HTTP requests
* JSON data handling
* Scheduled automation
* Gmail integration
* Dynamic expressions
* Automated email generation

## 🔮 Future Improvements

Possible enhancements include:

* Add multiple quote APIs as fallback sources
* Add personalized quotes based on user preferences
* Support multiple recipients
* Add inspirational images
* Store previously sent quotes to avoid repetition
* Add error handling and retry mechanisms
* Add Telegram or WhatsApp notifications
* Create a dashboard to monitor workflow executions

## 👩‍💻 Author

**Pooja Reddy**

GitHub: [@poojareddy24817](https://github.com/poojareddy24817)

---

⭐ If you find this project useful, consider giving the repository a star!
