# 1. Problem Statement

The objective of this workflow is to automate the process of receiving a **form submission**, processing the submitted data using an **AI Agent (powered by Google Gemini Chat Model)**, and then sending the AI-generated response to a specified email address.

This setup enables:
- AI-processed responses based on form input  
- Automated emailing workflow  
- End-to-end processing without manual effort  

---

# 2. Step-by-Step Process

## **Initial Setup**
1. Go to: https://www.n8n.io  
2. Create an account or log in if you already have one.  
3. Create a **new workflow** inside your personal workspace.

---

## **Creating the AI-Powered Email Workflow**

1. Add the trigger node **On Form Submission**.  
   - This node activates every time a user submits a form connected to your n8n instance.

2. Add an **AI Agent** node.  
   - This node will process the form submission using an LLM.  
   - It will generate meaningful and structured output.

3. Add the **Google Gemini Chat Model** node.  
   - Connect it to the **Chat Model** input of the AI Agent.  
   - Authenticate using Google credentials.  
   - Select the appropriate Gemini model.

4. Add a **Send Email** node (Gmail).  
   - Configure your Gmail credentials.  
   - Set recipient, subject, and content to use the AI Agent’s output.

5. Connect the nodes in the flow:
   - Form Submission → AI Agent → Gmail Send Message

6. Save the workflow.  
7. Click **Execute workflow** to test.  
8. Confirm that the email arrives in the inbox with the AI-generated content.

---

# 3. Implementation Screenshot

Below is the workflow that you created and executed:

<img width="1920" height="1032" alt="⚠️ My workflow 3 - n8n - Google Chrome 22-11-2025 11_35_46" src="https://github.com/user-attachments/assets/536a67c7-235b-44bd-b9ac-0400335d817e" />


---

# 4. Output Screenshot

The following email was received as a result of the workflow execution:

<img width="1920" height="1032" alt="Here&#39;s the information - sanjaynewbie2@gmail com - Gmail - Google Chrome 22-11-2025 11_11_06" src="https://github.com/user-attachments/assets/a09b9093-21f9-4936-86f5-f0ff133ddbc1" />

---

# 5. Summary / Learning Outcome

From this workflow, you learned:

- How to use the **On Form Submission** trigger in n8n  
- How to integrate an **AI Agent** with the **Google Gemini Chat Model**  
- How to automate email sending with Gmail inside n8n  
- How to build an end-to-end automation pipeline combining forms → AI → email  
- How AI can convert raw form data into meaningful, structured output  

This workflow can be extended to create chatbots, smart form responders, automated reporting systems, and more.

---
