# AI Email Reply Agent

An automated email reply agent built using **n8n** and **Google Gemini AI**.

This workflow reads unread emails from Gmail, generates professional replies using AI, stores the interaction in Airtable, and sends responses automatically.

---

## Architecture

Email Inbox → n8n Workflow → Gemini AI → Airtable Record → Email Reply

---

## Features

- Automatically fetches unread emails
- Uses Gemini AI to generate professional replies
- Stores email data and AI response in Airtable
- Automatically replies to the sender
- Runs on a scheduled interval

---

## Workflow Steps

1. **Schedule Trigger**  
   Checks for unread emails periodically.

2. **Fetch Emails**  
   Retrieves unread messages from Gmail.

3. **Get Email Details**  
   Extracts sender, body, and thread information.

4. **AI Response Generation**  
   Gemini AI generates a professional email reply.

5. **Maintain Records**  
   Stores email details and AI reply in Airtable.

6. **Mark Email as Read**

7. **Send Reply**

---

## Tech Stack

- n8n (workflow automation)
- Gmail API
- Google Gemini AI
- Airtable

---

## Setup

1. Import `myworkflow.json` into n8n
2. Connect your Gmail account
3. Add your Gemini API credentials
4. Connect Airtable
5. Activate the workflow

---

## Notes

- API keys and credentials are not included in the workflow export.
- You must configure your own credentials in n8n before running the workflow.

---

## License

This project is for learning and automation experimentation.