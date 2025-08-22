# SourceBot - Intelligent Knowledge Chatbot (RAG-based)

An **AI-powered chatbot** that uses Retrieval-Augmented Generation (RAG) to answer user questions with precise, source-backed responses.  
The chatbot indexes documentation and FAQs, enabling instant query resolution that is transparent and reliable.  
Built with **LangChain, Pinecone, and OpenAI API**, and deployed via **Streamlit** for an intuitive user experience.

---

##  My Role
I designed and implemented this project end-to-end:
- Built the RAG pipeline to combine document retrieval with generative AI.
- Authored the **PRD** to define chatbot features and roadmap.
- Scoped user personas and prioritized MVP functionality using **MoSCoW**.
- Conducted **A/B testing** of chatbot tones (formal vs conversational).
- Deployed a working prototype on **Streamlit** for interactive testing.

---

## ⚙ Technical Execution
1. **Document Indexing**  
   - Collected and processed FAQs, product manuals, and internal notes.  
   - Embedded documents into a **Pinecone vector database** using HuggingFace embeddings (`all-MiniLM-L6-v2`).  

2. **RAG Pipeline**  
   - Implemented retrieval using LangChain → top-k context passages.  
   - Combined retrieved context with queries for **OpenAI API** completion.  
   - Ensured transparency by attaching **source citations** to each answer.  

3. **Prototype Deployment**  
   - Built a **Streamlit app** with:  
     - Query input box.  
     - Conversational responses with **citations**.  
     - Confidence score and “copy response” option.  
   - Logged queries and responses for later analysis.  

---

##  Product Workflow
- Drafted a **PRD** defining MVP features:  
  - Must-have → Document search + cited answers.  
  - Should-have → Confidence scores.  
  - Could-have → Multi-turn memory + analytics dashboard.  
- Defined **user personas**:  
  - Support agents (faster ticket resolution).  
  - PMs (quick spec lookups).  
  - Developers (API reference queries).  
- Prioritized usability and speed for MVP launch.  

---

##  Data-Driven Decision Making
- Collected logs of chatbot queries and analyzed error cases.  
- Ran **A/B testing** comparing:  
  - **Formal style** (knowledge-base tone).  
  - **Conversational style** (friendly assistant).  
- Metrics tracked:  
  - Query resolution accuracy.  
  - Avg. resolution time.  
  - User satisfaction (1–5 feedback rating).  
- Findings: Conversational tone improved satisfaction **+18%**, while formal style reduced errors for technical queries.  
- Adopted a **hybrid approach** based on context.  

---

##  User-Centric Development
- Conducted pilot usability tests with 10 peers.  
- Feedback:  
  - “I want to see where the answer comes from.”  
- Iteration:  
  - Added **source highlighting + citation links**.  
- Result: Trust in chatbot responses increased significantly, with **85%+ satisfaction score** in testing.  

---

##  Key Features
- Ask questions in plain English.  
- Retrieves relevant documents + generates accurate responses.  
- Transparent answers with **source citations**.  
- **Confidence scores** for response reliability.  
- Deployed via **Streamlit** for easy access.  

---

##  Tech Stack
- **Python**: pandas, numpy, langchain  
- **Vector DB**: Pinecone (or FAISS for local)  
- **LLMs**: OpenAI GPT API  
- **Frontend/UI**: Streamlit  
- **Deployment**: Docker, Render/Heroku/AWS

## Disclaimer

This chatbot is for educational and internal productivity purposes.
It is not a substitute for professional or regulatory advice.
