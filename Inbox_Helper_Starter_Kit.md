# 📧 Inbox Helper Starter Kit

**Goal:** Help you manage email clutter locally with Open WebUI + AnythingLLM.

## What you need
- A computer (Windows, Mac, or Linux)
- Open WebUI installed (via Docker or local setup)
- Gmail or another email provider that supports IMAP

## Steps
1. **Connect your inbox**
   Configure the IMAP plugin with your email + app password.

   ```yaml
   tools:
     - name: "gmail_inbox"
       type: "imap"
       config:
         host: imap.gmail.com
         port: 993
         username: "your_email@gmail.com"
         password: "your_app_password"
   ```

2. **Import a Starter Prompt**

   ```
   You are my Inbox Helper. Your job:
   - Check my emails.
   - Flag important messages from school or bills.
   - Summarize key details in bullet points.
   - Ask me if I want a reminder.
   ```

3. **Run your first test**
   Ask: *"Check if I have any new emails from my child’s school and summarize them."*

## Next Step
Add automation (e.g., Power Automate or Zapier) to run this agent daily.
