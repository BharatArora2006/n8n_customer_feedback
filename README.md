# AI-Powered Customer Feedback Agent
This project demonstrates the creation of an intelligent agent that automatically categorizes customer feedback and triggers appropriate follow-up actions, streamlining workflows and improving customer experience.

## Overview
The AI Agent processes customer feedback submitted through a form and utilizes a Large Language Model (LLM) from GROQ to analyze the sentiment and intent. Based on the analysis, the agent categorizes the feedback as a Complaint, Compliment, or New Feature Request and initiates specific automated responses and actions.

**Here's how it works:**
1.  **Feedback Capture:** Customers submit their feedback via an online form.
2.  **LLM-Powered Analysis (GROQ):** The submitted feedback is sent to the GROQ LLM for analysis. The LLM determines the category of the feedback:
    * Complaint
    * Compliment
    * New Feature Request
3.  **Automated Response & Action:** Based on the identified category, the following actions are automatically triggered:
    * **Complaint:**
        * An apology email is sent to the customer via Gmail.
        * The complaint details are routed to the relevant team on Slack.
    * **Compliment:**
        * A thank-you email is sent to the customer via Gmail.
        * The positive feedback is shared with stakeholders on a dedicated Slack channel.
    * **Feature Request:**
        * An acknowledgment email is sent to the customer via Gmail.
        * The feature request is sent to the product/developer team on Slack.

## Tech Stack
This project leverages the following technologies:
* **Workflow Automation:** [n8n](https://n8n.io/) - Used as the workflow automation engine to orchestrate the data flow, LLM calls, and trigger actions.
* **Large Language Model (LLM):** [GROQ](https://groq.com/) - Powers the analysis and categorization of customer feedback.
* **Database:** [Airtable](https://www.airtable.com/) - Used to store and manage customer feedback data (potentially).
* **Email:** [Gmail](https://mail.google.com/) - Used for sending automated email responses to customers.
* **Messaging:** [Slack](https://slack.com/) - Used for internal communication and routing feedback to relevant teams.

**Note:** Due to the demo nature and potential limitations of trial versions, the live demo might be deactivated in the future.

## Learning Journey
This project was built as a learning exercise to explore and integrate the following tools: n8n, GROQ, Airtable, Gmail, and Slack. It was a rewarding experience to see these technologies come together to create a functional automated solution.
