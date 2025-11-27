🌍 Overview

Agents for Good is an AI-powered multi-purpose assistant designed to create real social impact.
The project demonstrates how AI agents can support:

Education

Mental wellness

Environmental awareness

NGO and charity coordination

Community empowerment


This repo contains the code, tools, RAG data, workflow, and demo files used to build the project.


---

🎯 Project Goals

Build a safe, helpful, and grounded AI agent

Show real-world use cases for social good

Demonstrate planning, tool-calling, memory, and RAG

Provide outputs and demos for judges and the community

Enable users with no coding experience to run a social-impact agent



---

🧠 Features

✔ Multi-step Task Planning

Breaks user queries into smaller steps and executes them autonomously.

✔ Tools Included

Task Manager Tool

Calculator Tool

(Optional) Poster/Message Creator

RAG Document Retriever (FAISS)


✔ RAG-Enabled

Retrieves answers from project documents (education notes, awareness tips, NGO guidelines, etc.).

✔ FastAPI Endpoint

Simple /agent endpoint for easy testing and deployment.

✔ Beginner-Friendly

Designed to run locally with minimum setup.


---

📁 Repository Structure

agents-for-good/
│
├── agent.py                 # Main agent logic
├── tools.py                 # Task and calculation tools
├── build_faiss.py           # RAG index builder
├── app.py                   # FastAPI app (optional)
│
├── data/
│   ├── notes.txt            # Grounding data
│   ├── docs.txt             # RAG documents
│   ├── faiss.index          # Generated FAISS index
│   └── faiss_docs.pkl       # Document mappings
│
├── poster/
│   └── agents-for-good.png  # Project poster
│
├── demo/
│   ├── screenshots/         # Execution screenshots
│   ├── output_examples.txt
│   └── demo_video_link.txt
│
└── README.md


---

🔧 Installation

1️⃣ Clone the repo

git clone https://github.com/sandeep-chaudhary/agents-for-good
cd agents-for-good

2️⃣ Install dependencies

pip install -r requirements.txt

(If requirements.txt not added yet, typical deps are:)

fastapi
uvicorn
faiss-cpu
sentence-transformers
numpy

3️⃣ Prepare RAG Index

python build_faiss.py

4️⃣ Run Agent Locally

python agent.py

5️⃣ Run FastAPI (optional)

uvicorn app:app --reload


---

🧪 Example Queries

Try these when running the agent:

“Give me a daily eco-friendly habit.”

“Add a task: prepare NGO awareness script.”

“Calculate my monthly savings.”

“Summarize the document about student motivation.”

“Plan a 7-day learning routine.”



---

🖼️ Poster

The project poster is included inside:

/poster/agents-for-good.png

This explains the idea visually for judges and the community.

