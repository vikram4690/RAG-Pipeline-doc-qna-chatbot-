# Classmate AI: Document Q&A Chatbot  

This project is an **AI-powered chatbot** that allows you to upload **PDF, DOCX, or TXT documents** and ask questions in natural language.  
It retrieves relevant chunks from your documents using **FAISS vector search** and generates answers using the **Groq LLM API**.  

---

## Features  

-  Upload **multiple documents** (`.pdf`, `.docx`, `.txt`)  
-  Document text automatically split into **chunks** for better retrieval  
-  Semantic search with **SentenceTransformers embeddings + FAISS**  
-  Conversational Q&A with **Groq API (Mistral model)**  
-  Clean and interactive **Gradio UI**  

---

##  Workflow  

1. **Upload Documents** (PDF/DOCX/TXT)  
2. **Extract & Preprocess Text** using `PyPDF2`, `python-docx`, and text splitter  
3. **Vectorize Chunks** with `sentence-transformers/all-MiniLM-L6-v2`  
4. **Build FAISS Index** for semantic similarity search  
5. **Answer Questions** using context + conversation history + Groq LLM (`mistral-saba-24b`)  
6. **Chatbot UI** with memory powered by Gradio  

---

##  Getting Started  

### 1. Clone Repository  
```bash
git clone https://github.com/your-username/doc-qna-chatbot.git
