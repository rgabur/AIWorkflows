🚀 Features

AI-driven appointment extraction
Automatically identifies:

Client name

Email address

Date & time

Meeting purpose

Google Calendar Integration
Creates events automatically with:

Title

Time & date

Guest email

Description

Reminders (if configured)

Automated email confirmation
Sends personalized confirmation emails to clients with full meeting details.

End-to-end automation
From receiving message → extracting details → calendar event → confirmation email.

Fully customizable
All nodes (AI, Email, Google Calendar, Templates) can be modified easily.

🛠️ Tech Stack

n8n – Workflow orchestration

AI/LLM Node – Extracting structured appointment details

Google Calendar Node – Creating calendar events

Email Node – Sending confirmation emails

Webhook / Trigger Node – Entry point for appointment requests

📂 Workflow Overview

Trigger Input
Workflow receives an appointment request (text message, form input, API call, etc.).

AI Node
Extracts meaningful fields from free-text messages.

Field Validator
Ensures required details (email, date, time) are present.

Google Calendar Node
Automatically creates a calendar event with:

Title

Date & Time

Description

Guest email

Email Confirmation Node
Sends a client confirmation containing all booking details.

▶️ How to Use

Import the workflow

Download the JSON file from this repository

Go to n8n → Import from File

Configure Google Calendar

Add Google OAuth2 credentials

Select the calendar where events should be created

Set up Email credentials

SMTP / Gmail / Outlook

Add sender name & email

Add AI API key

Update the AI/LLM node with your provider key

Activate and test the workflow

📧 Example Output Email
Subject: Your Appointment is Confirmed

Hello <Client Name>,

Your appointment has been successfully scheduled and added to your calendar.

📅 Date: <Date>  
⏰ Time: <Time>  
📌 Purpose: <Meeting Purpose>  
📍 Calendar: Google Calendar Event Created

Regards,  
AI Appointment Assistant
