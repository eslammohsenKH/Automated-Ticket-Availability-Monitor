# 🎟️ Automated Ticket Availability Monitor

An automated **n8n workflow** that monitors Ticketmaster events and sends instant notifications through **Telegram** and **Email** when a target event becomes available for sale.

---

## 📌 Project Overview

This project demonstrates an automated event-monitoring system built with **n8n** and the **Ticketmaster API**.

The workflow retrieves event data, normalizes the API response, filters events based on predefined criteria, checks ticket availability, and sends notifications when a matching event has an **onsale** status.

---

## 🎯 Business Objective

The main objective is to reduce the need for manually checking ticket availability.

The workflow allows users to define specific monitoring criteria and automatically identify matching events when the workflow is executed.

This approach can be adapted to monitor:

- Concerts
- Sports events
- Theater shows
- Conferences
- Other ticketed events

---

## ⚙️ Workflow

```text
Manual Trigger
      ↓
Ticketmaster API
      ↓
Normalize Events
      ↓
Monitoring Settings
      ↓
Filter Target Event
      ↓
Check Status = ON SALE
      ↓
 ┌───────────────┐
 ↓               ↓
Telegram        Email
Notification    Notification
