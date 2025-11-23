
- # Attendance Email Automation – n8n Workflow Documentation

## 1. Problem Statement

The goal of this workflow is to automate the process of sending emails whenever a user submits a form.  
This automation:

- Collects form submission data  
- Sends the data to Google Gemini Chat Model for processing  
- Uses an AI Agent to generate a refined response  
- Automatically sends the final message to the user's email through Gmail  

This reduces manual effort and ensures fast, accurate, and consistent communication.

---

## 2. Step-by-Step Process

### **Step 1 — On Form Submission (Trigger Node)**
- Workflow begins with the **"On form submission"** trigger node.  
- Whenever a form is submitted, n8n collects the form fields and passes them to the next node.

### **Step 2 — Google Gemini Chat Model**
- The form data is sent to the **Google Gemini Chat Model**.  
- The model processes the input and generates structured, meaningful information.  
- This output is given to the AI Agent.

### **Step 3 — AI Agent**
- The **AI Agent** receives both the form data and the Gemini model’s response.  
- It converts them into a final message.  
- The message is prepared in a format suitable for emailing.

### **Step 4 — Gmail: Send a Message**
- The AI Agent output is connected to the **Gmail "Send a message"** node.  
- The email includes:
  - Recipient email (from form field)
  - Subject
  - AI-generated content  
- The email is sent automatically.

---

## 3. Implementation Screenshot

<img width="1177" height="554" alt="Screenshot 2025-11-23 111605" src="https://github.com/user-attachments/assets/e286f672-239d-4ce1-9341-872420f3e686" />


---

## 4. Output Screenshot

> Replace the below placeholder with your actual screenshot of the Gmail received message.

```md
![Output Screenshot](your-output-image.png)

