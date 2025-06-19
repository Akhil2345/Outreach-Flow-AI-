# 🤖 Outreach‑Flow‑AI – Automate Influencer Outreach & CRM Sync

**AI‑Powered. Personalized. Scalable.**  
A LangChain‑based multi‑agent system that drafts, sends, and tracks influencer outreach emails while pushing every lead & reply into your favourite CRM.

> 🔧 Built for growth teams & founders who want to scale collaborations without repetitive manual work.

---

## ✨ What It Does

✅ Scrapes / imports influencer data (CSV, API, Notion)  
✅ Generates highly‑personalised cold emails with an LLM  
✅ Sends mail via Gmail / SMTP and logs delivery status  
✅ Captures replies, scores leads, schedules follow‑ups  
✅ Syncs everything to HubSpot / Notion / Airtable CRM

---

## 🔁 Example Workflow

1. 📄 Upload a CSV of influencer handles  
2. 🤖 Agent 1 enriches profiles & writes custom outreach copy  
3. ✉️ Agent 2 sends the email and waits for a response  
4. 🏷  Agent 3 tags replies and updates your CRM record  
5. 🔁 Agent 4 triggers a follow‑up if no reply in X days

---

## 🧱 Tech Stack

- 🧩 **LangChain** (agent orchestration)  
- 🦙 **Mistral LLM** via **Ollama** (local) or OpenAI API  
- ✉️ **smtplib / Gmail API** (mail delivery)  
- 📇 **Notion / HubSpot / Airtable SDKs** (CRM sync)  
- 🐍 **Python 3.10+**

---

## ⚙️ Setup

```bash
# 1. Clone this repo
git clone https://github.com/yourusername/Outreach-Flow-AI.git
cd Outreach-Flow-AI

# 2. Create & activate a virtual environment
python -m venv venv && source venv/bin/activate   # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. (Local mode) Make sure Mistral is running
ollama run mistral     # or set OPENAI_API_KEY for cloud LLM

# 5. Configure your SMTP / CRM keys in config.py, then launch
python main.py
