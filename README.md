# 📅 Habit Reminder Bot — n8n Automation

![n8n](https://img.shields.io/badge/n8n-Automation-orange)
![Telegram](https://img.shields.io/badge/Notification-Telegram-blue)
![Automation](https://img.shields.io/badge/Workflow-Scheduled-green)
![JavaScript](https://img.shields.io/badge/Code-Expressions-yellow)
![License](https://img.shields.io/badge/license-MIT-green)

An automated habit reminder workflow built using **n8n** and **Telegram Bot API**.

This system automatically runs on a scheduled time, generates a personalized daily habit checklist with dynamic date information, formats the reminder message, and delivers it directly to Telegram.

**Stack:**  
n8n · Schedule Trigger · Telegram Bot API · n8n Expressions · Workflow Automation


---

# 🎯 Project Overview


## Problem

Maintaining daily habits consistently can be challenging without proper reminders.

Common challenges include:

- Forgetting daily routines
- Lack of consistent tracking
- Manual reminder creation
- Difficulty maintaining productivity habits
- No automated accountability system


Common examples:

- Study schedules
- Exercise routines
- Reading goals
- Health habits
- Personal development activities


---

## Solution

This project creates an automated personal productivity assistant by:


1. Running a scheduled workflow every day
2. Generating a personalized habit checklist
3. Adding the current date automatically
4. Formatting the reminder message
5. Sending the checklist through Telegram


The workflow acts as a simple digital habit assistant that helps maintain consistency through automated reminders.


---

# ✨ Features


## Reminder Automation

✅ Daily scheduled execution  
✅ Automatic habit checklist generation  
✅ Personalized reminder messages  
✅ No manual triggering required  


## Message Processing

✅ Dynamic date generation  
✅ n8n expression usage  
✅ Custom message formatting  
✅ Structured notification format  


## Notifications

✅ Telegram instant delivery  
✅ Mobile-friendly reminders  
✅ Real-time habit notifications  


## Cost Efficiency

✅ No external APIs required  
✅ No paid services required  
✅ Lightweight automation workflow  


---

# 🗺️ System Architecture


```mermaid
flowchart TD

A["⏰ Schedule Trigger"]

--> B["⚙️ Edit Fields (Set)"]


B --> C["📅 Generate Habit Message"]


C --> D["📱 Telegram Notification"]

````

---

# 🏗️ Workflow Implementation

# Workflow 1: Daily Habit Reminder Pipeline

## Node 1 — Schedule Trigger

### Purpose

Automatically starts the reminder workflow at a configured time every day.

Example Configuration:

```text
Trigger:

Every Day


Time:

07:00 AM
```

Execution Flow:

```text
Scheduled Time

      ↓

Generate Reminder

      ↓

Send Telegram Message
```

---

# Node 2 — Edit Fields (Set)

### Purpose

Creates and formats the daily habit reminder message.

The node generates:

* Habit checklist
* Current date
* Motivational message
* Telegram-ready format

Example Output:

```text
📅 Daily Habit Reminder


Today's Habits


📚 Study for 1 hour

💧 Drink 8 glasses of water

🏃 Exercise for 30 minutes

📖 Read 20 pages

🧘 Meditate for 10 minutes


📅 Date:

July 02, 2026


💪 Small progress every day leads to big results.


🤖 Generated automatically using n8n.
```

---

# Node 3 — Telegram Notification

### Purpose

Deliver the formatted habit reminder directly to the user's Telegram account.

Processing:

```text
Habit Data

      ↓

Formatted Message

      ↓

Telegram Delivery
```

Example:

```text
📅 Daily Habit Reminder


📚 Study

💧 Hydration

🏃 Exercise

📖 Reading

🧘 Meditation


Have a productive day! 🚀
```

---

# 🔐 Credentials Required

| Service          | Purpose            |
| ---------------- | ------------------ |
| Telegram Bot API | Send reminders     |
| n8n Instance     | Workflow execution |

---

# ⚙️ Setup Guide

## 1. Configure Schedule Trigger

Set your preferred reminder time.

Example:

```text
Daily

07:00 AM
```

Test workflow execution.

---

## 2. Configure Habit Message

Edit the Set node.

Customize:

```text
Habit List

Motivational Message

Reminder Format
```

Example:

```text
Study

Exercise

Reading

Water Intake
```

---

## 3. Configure Telegram Bot

Steps:

1. Create a Telegram bot using BotFather
2. Copy bot token
3. Add Telegram credentials in n8n
4. Configure chat ID

---

## 4. Import Workflow

Import:

```text
workflow.json
```

Configure:

* Schedule time
* Habit checklist
* Telegram credentials

Activate workflow.

---

# 🧪 Testing Checklist

| Test Case             | Expected Result        |
| --------------------- | ---------------------- |
| Schedule executes     | Workflow starts        |
| Set node runs         | Reminder generated     |
| Date expression works | Current date displayed |
| Telegram executes     | Reminder received      |
| Workflow completes    | Successful execution   |

---

# 📁 Repository Structure

```text
Habit-Reminder-Bot-n8n/

│
├── README.md
│
├── workflow.json
│
├── screenshots/
│
│   ├── workflow.png
│   ├── schedule-trigger.png
│   ├── edit-fields.png
│   ├── telegram-output.png
│   └── workflow-execution.png
│
└── LICENSE
```

---

# 📸 Screenshots

Recommended screenshots:

* Complete workflow
* Schedule Trigger configuration
* Edit Fields message generation
* Telegram reminder output
* Workflow execution result

---

# 🚀 Future Improvements

| Feature                     | Implementation               |
| --------------------------- | ---------------------------- |
| Google Sheets Integration   | Store habit history          |
| Habit Completion Tracking   | Track completed tasks        |
| Custom Habit Database       | Manage habits dynamically    |
| Multiple Reminders          | Morning/night reminders      |
| Weekday Scheduling          | Different routines           |
| Google Calendar Integration | Calendar-based habits        |
| Weekly Reports              | Productivity summaries       |
| AI Habit Coach              | Generate personalized advice |

---

# 🎓 Skills Applied

## Automation

* n8n Workflow Automation
* Scheduled workflows
* Productivity automation

## Integrations

* Telegram Bot API
* Notification systems

## Programming

* n8n Expressions
* Dynamic data generation
* Message formatting

## Workflow Design

* Low-code automation
* Event scheduling
* Process automation

## Personal Productivity

* Habit tracking systems
* Reminder automation
* Digital assistants

---

# 📚 Learning Objectives

This project demonstrates:

* Building scheduled automation workflows
* Creating Telegram-based notification systems
* Using n8n expressions for dynamic content
* Designing lightweight productivity tools
* Automating repetitive personal tasks

---

# 🙌 Acknowledgements

* n8n
* Telegram Bot API

---

# 👨‍💻 Author

**Belio C. Sinangote**

BS Information Technology Student
Cebu Technological University (CTU)

GitHub:

[https://github.com/belioautomation](https://github.com/belioautomation)

This project is part of my **30-Day n8n Automation Portfolio**, showcasing practical automation solutions using **n8n, Telegram integrations, and scheduled workflow automation**.

---

# 📄 License

MIT License

```
```
