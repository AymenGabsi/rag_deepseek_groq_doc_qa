# 🐋 DeepSeek-R1 - Document RAG (Retrieval-Augmented Generation)

## 📌 Overview

This project implements a **Retrieval-Augmented Generation (RAG) system** for **document-based question answering** using:

- **DeepSeek-R1** (via **Groq**) for fast & efficient AI-powered responses.
- **ChromaDB** for storing and retrieving document embeddings.
- **HuggingFace Embeddings** for vectorization.
- **Streamlit** for an interactive UI.

🔹 **Users can upload a PDF, process it into a vector database, and query it for answers!**

---

## 🚀 Features

- 📄 **Upload and process PDF documents** into a vector store.
- 🔍 **Retrieve relevant document sections** using ChromaDB.
- 💬 **Generate AI-powered answers** using DeepSeek-R1 via Groq.
- 🎛 **Interactive UI** built with Streamlit.

---

## 📂 Project Structure

```plaintext
/project-folder
│-- main.py                # Streamlit UI for user interaction
│-- rag_utility.py         # Core logic for document processing & retrieval
│-- config.json            # Stores API keys
│-- requirements.txt       # Required dependencies
```

---

## 🛠 Installation & Setup

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/AymenGabsi/rag_deepseek_groq_doc_qa.git
cd your-repo
```

### **2️⃣ Set Up a Virtual Environment**

```bash
python -m venv venv
source venv/bin/activate   # For macOS/Linux
venv\Scripts\activate     # For Windows
```

### **3️⃣ Install Dependencies**

```bash
pip install --upgrade pip setuptools wheel
pip install -r requirements.txt
```

### **4️⃣ Configure API Keys**

- Open **config.json** and replace `your_groq_api_key` with your actual **Groq API Key**:

```json
{
  "GROQ_API_KEY": "your_groq_api_key"
}
```

---

## ▶️ Running the Application

After setting up, launch the Streamlit app:

```bash
streamlit run main.py
```

This will open a web interface where you can:

1. **Upload a PDF**
2. **Ask questions** about its content
3. **Receive AI-generated answers** powered by DeepSeek-R1

---

## 🏗 How It Works

1. **Upload a PDF** file.
2. **Extract text** and convert it into **vector embeddings** using HuggingFace.
3. **Store embeddings in ChromaDB** for efficient retrieval.
4. **Retrieve relevant sections** from ChromaDB when a user asks a question.
5. **Send retrieved data to DeepSeek-R1 (Groq) LLM** for final answer generation.

---

## 📌 Technologies Used

- [**LangChain**](https://www.langchain.com/) for orchestrating LLM-based workflows.
- [**DeepSeek-R1**](https://deepseek.com/) via **Groq** for LLM-based response generation.
- [**ChromaDB**](https://www.trychroma.com/) for vector storage and retrieval.
- [**HuggingFace Embeddings**](https://huggingface.co/docs) for document vectorization.
- [**Streamlit**](https://streamlit.io/) for UI interaction.

---

## 🤖 Future Enhancements

- 🔄 **Support more document formats** (TXT, DOCX, HTML, etc.)
- 📊 **Improve retrieval accuracy** using hybrid search (BM25 + embeddings).
- 🎨 **Enhance UI** with real-time answer explanations.
- 🚀 **Optimize response speed** by caching retrieval results.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## ⭐ Contributing

Contributions are welcome! Feel free to fork this repository, submit issues, or create pull requests.

📧 **For inquiries, reach out via GitHub Issues.**

🚀 Happy Coding!


