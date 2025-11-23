# Execute Workflow Email Sender – n8n Documentation

## 1. Problem Statement

This workflow is designed to send an automated email whenever the workflow is manually executed.  
It is useful for:

- Sending test emails
- Triggering reminders manually
- Running admin-controlled email automation
- Quick debugging of email configurations

The workflow contains a simple trigger and a Gmail node to send a predefined message.

---

## 2. Step-by-Step Process

### **Step 1 — Trigger: When Clicking "Execute Workflow"**
- This workflow starts when the user manually clicks the **Execute Workflow** button in n8n.
- No external input is required.
- This trigger is useful for testing email flows and manual notifications.

### **Step 2 — Gmail: Send a Message**
- The Gmail node is used to send an automated email.
- You configure:
  - Receiver email address
  - Subject line
  - Body text
- Once the workflow runs, an email is instantly delivered to the chosen recipient.

---

## 3. Implementation Screenshot

<img width="687" height="285" alt="Screenshot 2025-11-23 113812" src="https://github.com/user-attachments/assets/c2124932-4806-476d-bc69-29e9b92152d4" />

---

## 4. Output Screenshot

> Replace this placeholder with your actual screenshot of the Gmail message received.

```md
![Output Screenshot](your-output-email.png)
