# RAG with FAISS and Gemini

This notebook demonstrates a simple **Retrieval-Augmented Generation (RAG)** pipeline using:

- 🧠 **Sentence-Transformers** for text embeddings
- 📦 **FAISS** for fast vector similarity search
- 🤖 **Gemini API** (Google Generative AI) for answering questions based on retrieved context

---

## 💡 How It Works

1. **Sentence Embedding**  
   Input sentences are converted to vector embeddings using `all-MiniLM-L6-v2`.

2. **FAISS Vector Store**  
   These embeddings are indexed using `faiss.IndexFlatL2` to allow similarity search.

3. **Query**  
   A new query (e.g., *"I adore kittens"*) is embedded and searched for the top-`k` closest sentences.

4. **Prompt Construction**  
   The most similar sentences are used as context to construct a prompt.

5. **Answer Generation**  
   The prompt is passed to the **Gemini 1.5** model, which generates a context-aware answer.

---

## 🛠️ Requirements

```bash
pip install faiss-cpu sentence-transformers google-generativeai
