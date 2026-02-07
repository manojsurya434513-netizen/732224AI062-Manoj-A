# 1. Problem Statement

The objective of this workflow is to automate the process of **reading data from Google Sheets**, validating it using an **IF condition**, and then appending the data into different Google Sheets based on the result.

This setup enables:
- Automatic data reading from sheets  
- Conditional data processing  
- Intelligent data routing  
- Organized data storage into separate sheets  

---

# 2. Step-by-Step Process

## **Initial Setup**

1. Open your browser and sign in to your **n8n workspace**.  
2. Click **Create Workflow** to start a new workflow.

---

## **Creating the Conditional Google Sheets Workflow**

1. Add the trigger node **Manual Trigger**.  
   - This allows you to manually execute the workflow for testing.

2. Add the node **Google Sheets (Read Rows)**.  
   - Configure credentials for Google Sheets.  
   - Select the spreadsheet and sheet name.

3. Add an **IF node**.  
   - Set a condition to evaluate the incoming data.  
   - Decide the rule for separating rows.

4. Add the **Google Sheets (Append Row)** node for TRUE condition.  
   - Configure the output sheet where valid data will be stored.

5. Add another **Google Sheets (Append Row)** node for FALSE condition.  
   - Configure a different sheet for invalid or unmatched data.

6. Connect the flow as follows:
   - Manual Trigger → Read Rows → IF  
   - IF (TRUE) → Append to Sheet A  
   - IF (FALSE) → Append to Sheet B  

7. Save the workflow.  
8. Click **Execute Workflow** to run the process.  
9. Verify that data is appended correctly to respective sheets.

---

# 3. Summary / Learning Outcome

From this workflow, you learned:

- How to read rows from Google Sheets using n8n  
- How to apply conditions using the IF node  
- How to route data based on logic  
- How to append data into different sheets  
- How to build basic automation using manual triggers  

This workflow can be extended for:
- Data validation systems  
- Sorting applications  
- ETL processes  
- Admin dashboards  
- AI-based filtering logic
