# 🎯 Automated Lead-Tracking & Notification Engine

An enterprise-ready automated lead capture, database management, and instant notification pipeline built with **Activepieces**, **Notion**, and **Telegram Bot API**.

This system automatically intercepts incoming business leads from webhook sources or form submissions, logs and organizes them inside a Notion CRM Database, and instantly dispatches structured lead alerts to sales/operations teams via Telegram.

---

## 🛠️ Tech Stack & Architecture

* **Orchestration Engine**: [Activepieces](https://www.activepieces.com/)
* **Database / CRM Source**: [Notion API](https://developers.notion.com/)
* **Real-time Alert Channel**: [Telegram Bot API](https://core.telegram.org/bots/api)
* **Protocol**: Webhooks / Activepieces Triggers & Actions

### 🔄 Data Flow
* **Incoming Lead Form / Webhook** ➔ *(New Lead Data)*
* **Activepieces Orchestrator**:
  1. **Notion API** *(Creates/Updates CRM Record & Database Logs)*
  2. **Telegram Bot API** *(Formats & Dispatches Instant Sales Alert)*

---

## 🎯 System Features & Capabilities

* **Instant Lead Capture**: Zero-latency logging of prospective customer inquiries into Notion.
* **CRM Automated Logging**: Keeps customer attributes (Name, Email, Service Needed, Status) neatly organized in a central Notion database.
* **Real-time Sales Alerts**: Sends high-priority, formatted Markdown notifications directly to team Telegram chats or channels.
* **Error Handling & Deduplication**: Ensures data integrity during batch lead ingestion without dropping records.

---

## 📖 How to Use (طريقة الاستخدام)

1. **Lead Ingestion**:
   * Any new lead submitted via your web form or webhook endpoint triggers the workflow automatically.

2. **Automated CRM Logging**:
   * Activepieces creates a new record in your Notion Lead Database with all customer contact details and sets the initial lead status.

3. **Instant Notification**:
   * The team receives a real-time Telegram message with full lead details and a direct link to the Notion CRM entry for immediate follow-up.

---

## 🚀 Setup & Installation (خطوات الإعداد)

1. **Notion CRM Setup**:
   * Create a Notion Database with required properties: `Lead Name` (Title), `Email` (Email), `Phone` (Phone Number), and `Status` (Select).

2. **Import Workflow**:
   * Import the corresponding `workflow.json` into your Activepieces workspace.

3. **Configure API Keys & Connections**:
   * Connect your **Notion Integration Token** and **Telegram Bot Credentials**.

4. **Publish**:
   * Test with a dummy lead payload, verify the Notion row creation and Telegram alert, then click **Publish**.

---

## ⚖️ Rights & License (حقوق الملكية والاستخدام)

* **Author**: Youssef Amr (جو)
* **Role**: Automation Specialist & Developer
* **License**: MIT License – Free to use, modify, and distribute with attribution to the original author.

---
© 2026 **Youssef Amr**. All rights reserved.
