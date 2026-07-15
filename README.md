# 🤖 ESP32 AI Chatbot Assistant using RAG, LangChain & Ollama

An AI-powered chatbot that allows users to interact with the **ESP32 Datasheet** using natural language. Instead of manually searching through hundreds of pages of technical documentation, users can simply ask questions, and the chatbot provides accurate, context-aware answers using **Retrieval-Augmented Generation (RAG)**.

---

## 📌 Project Overview

Technical datasheets are often lengthy and difficult to navigate, making it time-consuming for students, engineers, and developers to find specific information. This project solves that problem by building an intelligent chatbot capable of understanding user queries and retrieving relevant information directly from the official ESP32 datasheet.

The chatbot combines **semantic search**, **vector databases**, and **Large Language Models (LLMs)** to generate precise answers grounded in the official documentation.

---

# 🎯 Problem Statement

The ESP32 datasheet contains detailed information about hardware specifications, peripherals, communication protocols, power management, and electrical characteristics. Searching this information manually is inefficient and often leads to wasted time.

This project aims to simplify access to technical documentation through an AI-powered conversational interface.

---

# 🎯 Objectives

- Build an AI assistant for ESP32 documentation.
- Implement Retrieval-Augmented Generation (RAG).
- Perform semantic document search using vector embeddings.
- Generate accurate responses using a locally hosted LLM.
- Provide an easy-to-use web interface for users.

---

# 🚀 Features

- 📄 Chat with the ESP32 Datasheet
- 🤖 AI-generated technical answers
- 🔍 Semantic Search using FAISS
- 🧠 Retrieval-Augmented Generation (RAG)
- 💻 Runs completely on local machine
- 🌐 Interactive Streamlit interface
- ⚡ Fast document retrieval
- 🔒 Offline privacy (using Ollama)

---

# 🏗️ System Architecture

```
                 ESP32 Datasheet (PDF)
                          │
                          ▼
                 LangChain PDF Loader
                          │
                          ▼
                 Text Chunking
                          │
                          ▼
             Sentence Transformer Embeddings
                          │
                          ▼
                 FAISS Vector Database
                          │
User Question ───────────►│
                          ▼
              Similarity Search (Retriever)
                          │
                          ▼
                 Ollama Large Language Model
                          │
                          ▼
                  AI Generated Answer
                          │
                          ▼
                 Streamlit User Interface
```

---

# ⚙️ Technologies Used

| Category | Technology |
|----------|------------|
| Language | Python |
| Framework | LangChain |
| LLM | Ollama |
| Embedding Model | Sentence Transformers |
| Vector Database | FAISS |
| Frontend | Streamlit |
| PDF Loader | PyPDFLoader |
| PDF Processing | PyPDF |
| AI Pipeline | Retrieval-Augmented Generation (RAG) |

---

# 📂 Project Structure

```
ESP32-AI-Chatbot/
│
├── esp32_datasheet_en.pdf
├── espchatbot.ipynb
├── requirements.txt
├── README.md
└── assets/
```

---

# 🔄 Workflow

### Step 1
Load the ESP32 Datasheet using LangChain.

↓

### Step 2

Split the document into smaller text chunks.

↓

### Step 3

Generate vector embeddings using Sentence Transformers.

↓

### Step 4

Store embeddings inside FAISS.

↓

### Step 5

Receive user question.

↓

### Step 6

Retrieve the most relevant document chunks.

↓

### Step 7

Provide retrieved context to Ollama.

↓

### Step 8

Generate an accurate AI response.

↓

### Step 9

Display answer through Streamlit.

---

# 🧠 Retrieval-Augmented Generation (RAG)

Instead of asking the Large Language Model directly, the chatbot first searches the ESP32 datasheet for relevant information.

The retrieved document sections are then sent to the language model as context.

This improves:

- Accuracy
- Reliability
- Reduced hallucinations
- Context-aware responses

---

# 📊 ESP32 Hardware Highlights

The chatbot is trained on the official ESP32 Datasheet which includes information about:

- Dual-core Xtensa LX6 Processor
- 2.4 GHz Wi-Fi
- Bluetooth & Bluetooth Low Energy
- 520 KB SRAM
- GPIO Pins
- ADC
- DAC
- UART
- SPI
- I2C
- I2S
- PWM
- Touch Sensors
- Deep Sleep Mode
- Power Management
- Security Features
- Flash Memory
- Communication Interfaces

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/ESP32-AI-Chatbot.git
```

Go to project directory

```bash
cd ESP32-AI-Chatbot
```

Install dependencies

```bash
pip install -r requirements.txt
```

Start Ollama

```bash
ollama serve
```

Run your preferred model

```bash
ollama run llama3
```

Launch Streamlit

```bash
streamlit run app.py
```

---

# 💬 Example Questions

- What is ESP32?
- Explain GPIO pins.
- What is Deep Sleep mode?
- Difference between Wi-Fi and Bluetooth?
- Explain ADC.
- Explain UART.
- What are RTC GPIOs?
- What is PWM?
- What are ESP32 power modes?
- Explain touch sensors.

---

# 📈 Applications

- AI Documentation Assistant
- Technical Support Chatbot
- Embedded Systems Learning
- Engineering Education
- IoT Development
- Electronics Documentation Search
- Research Assistance

---

# 🎓 Learning Outcomes

During this project, I learned:

- Retrieval-Augmented Generation (RAG)
- LangChain Framework
- Vector Databases
- FAISS
- Semantic Search
- Prompt Engineering
- Ollama
- Streamlit Development
- Embedding Models
- Document Question Answering
- Large Language Models

---

# 🔮 Future Improvements

- Multi-document support
- Voice-based interaction
- Image understanding
- Chat history
- Cloud deployment
- User authentication
- Better UI/UX
- Support for multiple datasheets
- Citation-based responses
- PDF upload by users

---

# 📚 References

- Official ESP32 Datasheet
- Espressif Documentation
- LangChain Documentation
- Ollama Documentation
- FAISS Documentation
- Sentence Transformers Documentation
- Streamlit Documentation

---

# 👨‍💻 Author

**Dhruv Dhanraj Sawarkar**

B.Tech Electronics Engineering

Yeshwantrao Chavan College of Engineering (YCCE), Nagpur

---

## ⭐ If you found this project useful, consider giving it a Star!
