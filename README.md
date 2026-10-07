# 🤖 Retell AI Voice Agent – Google Calendar & Sheets Integration

An automated backend pipeline built on **Make.com** that connects an AI voice agent (Retell AI) with **Google Calendar** and **Google Sheets** for real-time scheduling and lead logging.

---

## 🔄 Workflow Architecture

```text
[ Custom Webhook / Retell AI ] ──► [ Router ]
                                       ├──► Route 1: [ Google Calendar: Search Events ] ──► [ Webhook Response (Availability) ]
                                       └──► Route 2: [ Google Calendar: Create Event ]  ──► [ Google Sheets: Add Row ] ──► [ Webhook Response (Confirmation) ]
