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
