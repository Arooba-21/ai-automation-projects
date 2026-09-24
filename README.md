# ai-automation-projects

## Workflow 01 — Lead Capture
### Gmail + Google Sheets Automation
* **Problem:** Manually tracking leads is time-consuming and error-prone.
* **Solution:** Upon form submission, data is automatically saved to Google Sheets and an email notification is sent.
* **Tools:** n8n Form Trigger, Google Sheets, Gmail
* **Learned:** Trigger → Action flow, passing data via expressions (`{{ $json.field }}`), and OAuth authorization.

### Screenshot

![lead capture(gmail google sheets workflow)](./Screenshots/lead%20capture(gmail%20google%20sheets%20workflow).PNG)

## Workflow 02 — Automated Lead Routing
### Switch-Based Gmail Automation
* **Problem:** Leads from different industries or departments are not automatically routed to the correct salesperson.
* **Solution:** Based on the department field in the form submission, a Switch node routes the lead to the appropriate branch (Tech/Finance/Sales), with each branch sending its own customized email.
* **Tools:** n8n Form Trigger, Switch node, Gmail (multiple instances)
* **Learned:** Conditional routing/branching logic, creating multiple independent output paths from a single trigger.

### Screenshot

![Automated Lead Routing(switch gmail workflow)](./Screenshots/Automated%20Lead%20Routing(switch%20gmail%20workflow).PNG)

## Workflow 03 — Lead → CRM Automation

* **Problem:** Manually entering lead data into a CRM is time-consuming and error-prone.
* **Solution:** Upon form submission, lead details (Name, Email, Phone, Company, Status) are automatically created as a record in Airtable CRM, and an instant email notification is sent out.
* **Tools:** n8n Form Trigger, Airtable (Create a record), Gmail
* **Learned:**
  * How APIs function (request/response workflows, authentication via API keys/OAuth).
  * Debugging field type mismatches (e.g., array vs. plain values, Airtable field types).
  * Understanding the difference between "Map Automatically" and "Map Each Column Manually".
  * Utilizing the Typecast option to automatically format incoming data types.
 
    
### Screenshot

![Airtable automation](./Screenshots/Airtable%20automation.PNG)

## Output
![Airtable output](./Screenshots/Airtable%20output.PNG)
