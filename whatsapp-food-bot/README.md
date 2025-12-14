# WhatsApp Food Ordering Bot (n8n + AI)

An AI-powered WhatsApp food ordering assistant built using **n8n**, **Google Gemini**, **Airtable**, and **WhatsApp Cloud API**.

This bot can:
- Take food orders via WhatsApp
- Check inventory before confirming orders
- Reject out-of-stock items automatically
- Answer FAQs from Airtable
- Store confirmed orders in Airtable
- Maintain conversation memory per user

---

## Tech Stack
- n8n (workflow automation)
- WhatsApp Cloud API
- Google Gemini (LLM)
- Airtable (Inventory, Orders, FAQ)
- ngrok (local webhook testing)

---

## Features
- Friendly WhatsApp-style conversation
- Inventory validation before asking quantity
- Automatic order confirmation / rejection
- FAQ search from Airtable
- Session-based memory per WhatsApp user

---

## Workflow Overview
1. WhatsApp Trigger receives message
2. AI Agent decides intent (order / FAQ / stock)
3. Inventory checked before order confirmation
4. Orders saved only if item is available
5. Response sent back to WhatsApp

---

## How to Use
1. Import `n8n-workflow.json` into n8n
2. Configure credentials:
   - WhatsApp Cloud API
   - Google Gemini API
   - Airtable Personal Access Token
3. Update phone number ID and webhook URL
4. Activate workflow

---

## Screenshots
## 🧠 Architecture Overview

![Workflow](screenshots/n8n-automation.png)

---

## 📦 Airtable Structure

### Inventory Table
![Inventory](screenshots/inventory-table.png)

### Orders Table
![Orders](screenshots/order-table.png)

### FAQ Table
![FAQ](screenshots/faq-table.png)

### Test
![Test](screenshots/test-output.jpg)

---

## Note
Secrets and API keys are **not included** in this repository.
