# 🤖 LLM Chatbot System (Stateful with LangGraph)

A conversational AI chatbot built using **Streamlit + LangGraph + HuggingFace LLM**.

This project demonstrates a **stateful chatbot**, where conversation history is maintained and used to generate more context-aware responses.

---

## 🚀 Features

* 💬 Interactive chat interface using Streamlit  
* 🧠 Context-aware responses using conversation memory  
* 🔗 LangGraph-based workflow for structured processing  
* 🤖 Powered by HuggingFace LLM (Llama 3.1)  
* ⚡ Clean and modular architecture  

---

## 🧱 Tech Stack

* **Frontend:** Streamlit  
* **LLM:** HuggingFace (`meta-llama/Llama-3.1-8B-Instruct`)  
* **Framework:** LangGraph + LangChain  
* **Environment Management:** python-dotenv  

---

## 📁 Project Structure
.
├── app.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md


---

## ⚙️ Setup Instructions

### 1. Clone the repository

git clone https://github.com/Venkatesh-Bollarapu/llm-chatbot.git

cd llm-chatbot

---

### 2. Create virtual environment

python3 -m venv venv
source venv/bin/activate

---

### 3. Install dependencies

pip install -r requirements.txt
---

### 4. Add API Key

Create a `.env` file in the root directory:

HUGGINGFACEHUB_API_TOKEN=your_huggingface_token_here

---

### 5. Run the app

streamlit run app.py

---

## 🧠 How It Works

1. User enters a message through the Streamlit UI  
2. Chat history is stored in `session_state`  
3. Messages are converted into LangChain format  
4. LangGraph processes the conversation flow  
5. HuggingFace LLM generates a response  
6. Response is displayed and added to history  

---

## 🔄 Chat Behavior

* This is a **stateful chatbot**
* Previous messages are **used as context**
* Enables **multi-turn conversations**

---

## ⚠️ Notes

* Requires a valid HuggingFace API token  
* Response quality depends on the selected model  
* Free-tier tokens may have rate limits  

---

## 🔮 Future Improvements

* Add persistent memory (database)  
* Integrate RAG (PDF / document QA)  
* Improve UI/UX (chat styling, loading indicators)  
* Deploy on Streamlit Cloud / HuggingFace Spaces  

---

## 👨‍💻 Author

**Venkatesh Bollarapu**
