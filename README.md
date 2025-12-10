# 📹 YouTube Summarizer & Q&A Bot  
**Summarize any YouTube video and ask questions about its content — powered by IBM watsonx.ai, LangChain, FAISS, and Gradio.**

This project automatically fetches a YouTube video transcript, summarizes it using an LLM, and allows users to ask follow-up questions. It uses **retrieval-augmented generation (RAG)** to provide accurate, context-aware answers grounded in the video.

---

## 🚀 Features

### ✅ 1. YouTube Transcript Extraction
- Automatically fetches the transcript (manual or auto-generated)
- Cleans and formats the text for processing

### ✅ 2. Video Summarization
- Uses IBM Watsonx LLM (Granite / Llama / Mistral depending on model selection)
- Generates a concise paragraph summary of the video

### ✅ 3. Question Answering (RAG Pipeline)
- Splits transcript into chunks using LangChain
- Embeds text with IBM SLATE embeddings
- Stores embeddings in a FAISS vector index
- Retrieves relevant chunks and generates answers with an LLM

### ✅ 4. Gradio Web App Interface
- Intuitive UI for summarization and Q&A  
- Paste a YouTube URL → summarize → ask questions

---

## 🛠️ Tech Stack

| Component | Technology |
|----------|------------|
| LLM | IBM watsonx.ai (Granite / Llama / Mistral models) |
| Embeddings | IBM SLATE embedding model |
| Vector Search | FAISS |
| Framework | LangChain / LangChain-IBM |
| UI | Gradio |
| Transcript Retrieval | youtube-transcript-api |

---
