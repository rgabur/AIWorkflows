🚀 Features
🤖 AI Chatbot Interaction

User sends a message (WhatsApp / Telegram / Website / API).

Chatbot understands natural language using an LLM.

Extracts:

Client name

Email address

Date & time

Purpose of meeting

📅 Google Calendar Integration

Automatically creates a meeting event with:

Title

Date & time

Guest email

Description

Optional Google Meet link (if enabled)

📧 Automated Email Confirmation

After booking, the chatbot sends a confirmation email with:

Meeting details

Calendar event info

Purpose of meeting

Any instructions or links

🔁 End-to-End Automation

User → Chatbot → AI Understanding → Calendar Event → Email Confirmation → Done.

🛠️ Tech Stack

n8n — workflow automation platform

LLM / AI Node — natural language understanding

Google Calendar Node — for event creation

Email Node (SMTP / Gmail) — for confirmation emails

Webhook / Chatbot Trigger — depending on platform (WhatsApp, Telegram, Webchat, etc.)

📂 Workflow Overview

Chatbot Trigger
User sends a message like:
"I want to book an appointment tomorrow at 3 PM to discuss my project."

AI Node
Extracts structured fields:

name

email

date

time

purpose

Validator
Ensures required fields exist.

Google Calendar Node
Creates an event automatically.

Email Confirmation Node
Sends a personalized confirmation email to the client.

▶️ How to Use
1. Import Workflow

Download the JSON from the /workflows folder.

Import into n8n using Settings → Import from File.

2. Connect Chatbot Trigger

Examples:

WhatsApp Cloud API

Telegram Bot

Webhook for website chat

3. Add Google Calendar Credentials

Set up OAuth and assign the target calendar.

4. Configure Email Node

Add SMTP / Gmail credentials.

5. Add AI API Key

Configure the LLM node (OpenAI / Groq / Claude / Gemini).

6. Activate Workflow

Test by sending the chatbot a sample appointment message.

📧 Example Confirmation Email
Subject: Your Appointment is Confirmed

Hello <Client Name>,

Your appointment has been successfully booked through our chatbot.

📅 Date: <Date>
⏰ Time: <Time>
📌 Purpose: <Purpose>
📍 Google Calendar event created

Regards,
AI Appointment Assistant
