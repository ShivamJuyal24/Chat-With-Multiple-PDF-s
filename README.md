# Chat With Multiple PDFs 🧠📄

A Streamlit-based web app that allows users to upload multiple PDFs and ask questions based on their content. It uses Google Generative AI and LangChain to extract and understand text, storing embeddings in a FAISS vector store for fast and relevant answers.

## 🔍 Features

- 📤 Upload and process multiple PDFs
- 🤖 Ask natural language questions
- 💡 Get context-aware answers from the documents
- ⚡ Fast search using FAISS and LangChain

## 🛠️ Built With

- [Streamlit](https://streamlit.io/)
- [LangChain](https://www.langchain.com/)
- [Google Generative AI](https://ai.google/)
- [FAISS](https://github.com/facebookresearch/faiss)

## ⚙️ How It Works

1. **📄 Upload PDFs**
   - Users can upload one or more PDF documents through the Streamlit interface.

2. **🧠 Text Extraction & Chunking**
   - The PDFs are read, and text is extracted.
   - Text is split into manageable chunks for better processing.

3. **📚 Embedding Generation**
   - Each chunk is converted into a numerical vector using Google Generative AI embeddings.
   - These embeddings capture semantic meaning.

4. **🗃️ Vector Storage (FAISS)**
   - All the vectors are stored in a FAISS vector database.
   - This allows for fast similarity search when users ask questions.

5. **❓ Ask a Question**
   - Users type a question related to the uploaded PDFs.

6. **🔎 Similarity Search**
   - The app finds the most relevant text chunks using vector similarity from FAISS.

7. **🧠 Answer Generation**
   - LangChain uses the relevant chunks and Google Generative AI to generate an accurate, context-aware response.

8. **💬 Response Display**
   - The app displays the answer directly in the chat-like interface.



## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.8+ installed.

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/Chat-With-Multiple-PDFs.git
cd Chat-With-Multiple-PDFs
```
2. **Set up a virtual environment (optional but recommended)**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. **Install dependencies**
```bash
pip install -r requirements.txt
```
4. **Create a .env file**
```bash
GOOGLE_API_KEY=your_google_gen_ai_key

```
5. **Run the App**
```bash
streamlit run app.py
```


## 📁 Project Structure
```
.
├── app.py                # Main Streamlit app
├── requirements.txt      # Python dependencies
├── .env                  # API keys (not included in version control)
├── faiss_index/          # Stores vector database for document search
└── venv/                 # Virtual environment (optional)
```

## 📸 Screenshots
---
![Screenshot 2025-04-26 001704](https://github.com/user-attachments/assets/2377b8f0-188c-47f8-be82-8c7ee3157f3f)

---

## 🙋‍♀️ Questions or Contributions?

Feel free to [open an issue](https://github.com/ShivamJuyal24/Chat-With-Multiple-PDFs/issues) or submit a pull request. Contributions, suggestions, and stars are always welcome!

---

Made with ❤️ by [Shivam Juyal](https://github.com/ShivamJuyal24)

