# 💬 AI Translation RAG Copilot & LQA Auditor

An open-source **Retrieval-Augmented Generation (RAG)** and **Localization Quality Assurance (LQA)** copilot designed for professional translators, localization engineers, and language service providers. 

Optimized to run smoothly on Google Colab using a free T4 GPU via 4-bit quantization, this tool bridges the gap between massive style guides/glossaries and real-time translation workflows.

Some example texts are provided for anyone to test the program.

---

## 🎯 Key Features

- **Interactive RAG Copilot:** Ask questions about style guides, formatting rules, or ambiguous glossary terms and get instant, citation-backed answers.
- **Automated LQA / QA Auditor:** Upload a Source PDF and a Target PDF (or paste text) to automatically audit translations block-by-block against the client's style guide, flagging terminology errors, formatting flaws, and stylistic violations.
- **Dynamic Domain-Specific Prompting:** Instantly adapt the system's persona and focus via a dropdown selector (*GameLoc & Software, Life Sciences/Medical, Legal & Financial, Technical/Industrial, or General*).
- **Dynamic Vector Store (FAISS):** Upload any custom PDF style guide or glossary on-the-fly directly from the Streamlit web interface.
- **Edge-Optimized LLM:** Powered by **Qwen 2.5 (7B-Instruct)** running locally in 4-bit NF4 precision alongside multilingial embeddings (`paraphrase-multilingual-MiniLM-L12-v2`).

---

## 🛠️ Tech Stack

- **Framework:** Streamlit, LangChain (LCEL)
- **Vector Database:** FAISS (Local Indexing)
- **LLM & Quantization:** Hugging Face Transformers, BitsAndBytes (`load_in_4bit`)
- **Environment:** Google Colab (T4 GPU) + Cloudflare Tunnels
