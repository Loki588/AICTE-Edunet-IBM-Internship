# Interview Trainer Agent – AI-Powered Interview Preparation System

This repository contains the implementation of the **Interview Trainer Agent**, developed as part of an academic internship project. The solution leverages **IBM Watsonx.ai**, **IBM Granite Foundation Models**, and **Retrieval-Augmented Generation (RAG)** to deliver a personalized and intelligent interview preparation experience.


# 📌 Project Overview

The **Interview Trainer Agent** is an AI-powered assistant designed to support candidates in preparing for job interviews. By analyzing the user's profile, job role, experience level, and resume input, the agent generates:

- Tailored interview questions  
- Model answers and improvement tips  
- HR guidelines and behavioral scenarios  
- Technical and soft skill assessments  

This agent enhances user confidence and readiness by simulating real-world interview scenarios using advanced AI techniques.


# 🧠 Technologies & Frameworks

- **IBM Watsonx.ai Agent Lab**  
- **IBM Granite-embedding-278m-multilingual** (for text embedding)  
- **LangGraph** (for agent orchestration)  
- **ReAct** architecture (Reasoning + Acting framework)  
- **Retrieval-Augmented Generation (RAG)**  
- IBM Cloud Lite (entirely within free-tier resources)


# ⚙️ Agent Configuration

| Component         | Configuration                          |
|------------------|----------------------------------------|
| AI Model          | `llama-3-3-70b-instruct`               |
| Framework         | LangGraph                              |
| Architecture      | ReAct                                  |
| Embedding Model   | `granite-embedding-278m-multilingual`  |
| Chunk Size        | 2000                                   |
| Chunk Overlap     | 200                                    |

# 🔧 Model Parameters

| Parameter            | Value  |
|----------------------|--------|
| Frequency Penalty    | 0      |
| Presence Penalty     | 0      |
| Temperature          | 0.7    |
| Top P (nucleus)      | 1      |
| Max Tokens           | 2000   |


# 📂 Knowledge Base Contents

The agent's knowledge retrieval is powered by the following custom-curated content files:

1. `interview_questions.txt` – Domain-specific technical questions  
2. `hr_guidelines.txt` – Standard HR procedures and expectations  
3. `behavioral_scenarios.txt` – STAR-based soft skill scenarios  
4. `industry_expectations.txt` – Job role and sector-specific expectations  
5. `model_answers.txt` – Ideal answers for common questions  
6. `technical_skills_list.txt` – Categorized technical competencies  

All files were uploaded into the Watsonx Agent Knowledge tab and indexed with proper chunking and multilingual embedding.


# 💬 Sample User Prompts

- “I am a fresher applying for a software role. Can you help me prepare?”  
- “Generate HR interview questions for a senior data analyst.”  
- “How should I respond to 'Tell me about a time you faced conflict at work'?”  


## 📑 Deployment Context

This project has been executed entirely within IBM Cloud Lite’s free-tier constraints, ensuring accessibility and cost-efficiency. The solution is suitable for integration into job prep platforms, career services, or educational portals
