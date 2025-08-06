# College Admission Agent (RAG-Based AI using IBM Cloud)

This project is an AI-powered College Admission Assistant that leverages Retrieval-Augmented Generation (RAG) with IBM Granite foundation models to help students get instant, accurate, and relevant responses to their admission-related queries.

> Built and deployed entirely using **IBM Cloud Lite**, **Watsonx.ai**, and **IBM Granite models** – no code or scripts required.

---

## Problem Statement

Prospective students often face delays and confusion in accessing admission information such as eligibility criteria, course offerings, fee structures, and deadlines. Manual query handling by admissions departments is time-consuming and prone to inconsistencies. 

There is a need for an AI-based solution that can:
- Understand natural language queries.
- Retrieve reliable information from official sources.
- Respond instantly with relevant details.

---

## Proposed Solution

We developed a **RAG-based AI agent** using IBM Watsonx.ai that:
- Uses uploaded institutional documents and official website data.
- Retrieves and summarizes relevant content.
- Uses IBM Granite LLM to generate accurate answers.
- Delivers real-time responses in natural language.

---

## System Development Approach

### IBM Services Used
- Watsonx.ai (Lite plan)
- Watsonx.ai Runtime Service
- Deployment Space
- File Tool (for .txt document retrieval)
- Web Tool (for scraping live data from the college site)

### Tools & Features
- **granite-3-3-8b-instruct** (foundation model)
- **Agentic Lab** interface (no coding needed)
- **Document chunking** for precise retrieval
- **Real-time web integration** for fresh content

---

## Deployment Steps

1. **Create IBM Cloud Account** and enable Watsonx.ai Lite service.
2. **Create Watsonx.ai Runtime Service**.
3. **Launch Watsonx.ai Agentic Lab** and build an AI Agent.
4. **Upload `.txt` documents** using File Tool.
5. **Add Web Tool** and link to the official college website.
6. **Select Granite model** for response generation.
7. **Create Deployment Space** and associate your Runtime.
8. **Deploy Agent** and test via Preview.

> Note: Deployment is only supported on **Pay-as-you-go (non-Lite)** plans due to runtime restrictions.

---

## Sample Output (Preview)

**User:** What is the eligibility for B.Tech in Computer Engineering?  
**Agent:** Candidates must have passed 10+2 with Physics & Mathematics, and possess a valid MHT-CET or JEE Main score. Minimum 45% marks required (40% for reserved category).

---

## Knowledge Base Source

- College Name: **Modern Education Society's Wadia College of Engineering (MESCOE)**
- Website: [https://mescoe.mespune.org](https://mescoe.mespune.org)
- Official documents extracted: eligibility criteria, departments, courses offered, fee structure, contact info

---

## References

1. [IBM Watsonx.ai Agentic Lab Documentation](https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-agent-lab.html)
2. [IBM Granite Foundation Models](https://www.ibm.com/granite)
3. [MESCOE Official Website](https://mescoe.mespune.org)

---
## 📌 Note

Due to IBM Cloud Lite plan limitations, deploying an agent as an AI service requires a **Pay-as-you-go** plan. Lite accounts will encounter `"status": 402, "message": "Invalid status during deploying the AI service"` during deployment. Please upgrade your plan to proceed.

---
