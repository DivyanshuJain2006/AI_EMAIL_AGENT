AI Email Agent

An AI-powered Email Agent built using LangGraph and LangChain that automates email drafting, reviewing, and sending through an interactive workflow.

Features

* Extract recipient details and email requirements.
* Generate professional email drafts using an LLM.
* Review generated emails before sending.
* Human-in-the-loop approval using LangGraph interrupts.
* Revise emails based on user feedback.
* Send emails using SMTP integration.
* Manage workflow state using LangGraph checkpointing.

Tech Stack

* Python
* LangGraph
* LangChain
* Groq LLM
* Pydantic
* SMTP
* SQLite

Project Structure

01_email_agent/
├── agent.py
└── send_email.py
requirements.txt
.gitignore
README.md

Installation

1. Clone the repository.
2. Create a virtual environment.
3. Install dependencies:

pip install -r requirements.txt

4. Create a .env file:

GROQ_API_KEY=your_api_key
EMAIL_ADDRESS=your_email
EMAIL_PASSWORD=your_app_password

5. Run the agent:

python 01_email_agent/agent.py

Workflow

User Input → Information Retrieval → Email Drafting → Human Review → Feedback / Approval → Email Sending

Future Improvements

* Better handling of missing user information.
* Persistent conversation memory.
* Gmail API integration.
* Improved error handling.
