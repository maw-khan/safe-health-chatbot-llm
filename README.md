# Safe Health Chatbot using LLMs
![Python](https://img.shields.io/badge/Python-3.10-blue)
![NLP](https://img.shields.io/badge/NLP-LLM-orange)
![Framework](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![Model](https://img.shields.io/badge/Model-FLAN--T5-green)
![Project](https://img.shields.io/badge/Status-Completed-brightgreen)
![Focus](https://img.shields.io/badge/Focus-AI%20Safety-red)

A safety-aware health query chatbot built using **Large Language Models (LLMs)**, prompt engineering, and controlled response generation.

---

## 📌 Overview

This project explores how to build a **safe and responsible AI chatbot** for answering general health-related questions using open-source LLMs.

Unlike typical chatbots, this system focuses on:

- Preventing unsafe medical advice
- Controlling model behavior through prompt engineering
- Adding a safety filtering layer
- Ensuring stable and predictable responses

---

## 🎯 Objectives

- Build a chatbot using an open-source LLM (FLAN-T5)
- Apply prompt engineering for behavior control
- Implement safety constraints for health-related queries
- Evaluate model reliability and limitations

---

## 🚀 Key Features

- 🧠 Instruction-based chatbot using FLAN-T5
- 🛡️ Safety-focused prompt engineering
- ⚠️ Rule-based filtering for risky health queries
- 🔒 Controlled text generation (deterministic decoding)
- 📊 Real-world testing and failure analysis
- 📉 Model limitation and safety evaluation

---

## 🧠 Why This Project Matters

Most chatbot projects focus only on generating responses.

This project focuses on:

> **How to control and constrain AI systems in safety-critical domains**

It demonstrates:
- Responsible AI design
- Understanding of LLM limitations
- Real-world AI system thinking (not just modeling)

---

## 🏗️ System Architecture

The chatbot system is designed with multiple layers to ensure safe and controlled behavior:
User Query
   ↓
Input Safety Filter
   ↓
Prompt Engineering Layer
   ↓
LLM (FLAN-T5)
   ↓
Controlled Response Generation
   ↓
Final Output
---

### 🔍 Component Breakdown

#### 1. Input Safety Filter
- Detects risky or sensitive queries
- Blocks unsafe inputs before reaching the model

#### 2. Prompt Engineering Layer
- Structures instructions to guide model behavior
- Enforces safety constraints within the prompt

#### 3. Language Model (FLAN-T5)
- Generates responses based on input prompt
- Instruction-tuned transformer model

#### 4. Controlled Generation
- Uses deterministic decoding (no randomness)
- Ensures stable and predictable outputs

---

### 🧠 Design Philosophy

Instead of relying only on the model, we designed a **multi-layer control system**:

> AI System = Model + Prompt + Safety + Control

This reflects how real-world AI systems are built.

---

## 🤖 Model Details

- Model: **FLAN-T5 (Base)**
- Source: HuggingFace Transformers
- Type: Instruction-tuned sequence-to-sequence model

---

### 📌 Why FLAN-T5?

FLAN-T5 is designed to:

- Follow natural language instructions
- Perform well on question-answering tasks
- Work efficiently on limited hardware (e.g., Google Colab)

---

### ⚠️ Model Limitations

- Not trained specifically for medical data
- Limited ability to enforce strict safety rules
- Can generate hallucinated or generic responses

---

## 📊 Results & Observations

The chatbot was tested on a variety of general and sensitive health-related queries.

### ✅ What Worked Well

- Able to respond to simple health-related questions
- Maintains safe behavior in certain cases
- Avoids strong medical claims when properly prompted

---

### ⚠️ Observed Issues

- Responses can be overly short or generic
- Sometimes produces irrelevant or incoherent outputs
- Struggles with complex or sensitive queries
- Limited understanding of context in some cases
  
---

## 🧠 Failure Analysis

During testing, several limitations were observed:

### 1. Hallucination
The model occasionally generates incorrect or nonsensical information.

### 2. Weak Instruction Following
Despite prompt constraints, the model does not always follow safety rules strictly.

### 3. Lack of Domain Knowledge
The model is not trained specifically on medical data, leading to vague or inaccurate responses.

### 4. Over-Simplification
To remain safe, the model often produces overly generic answers.

---

### 📌 Key Insight

> Prompt engineering improves behavior, but cannot fully control model outputs.

This highlights the importance of:
- Model selection
- Fine-tuning
- External knowledge integration

---

## 🔧 Improvements Implemented

To address the observed issues, the following improvements were introduced:

### 🛡️ Safety Filtering Layer
- Blocks risky queries before model processing

### 🎯 Prompt Optimization
- Structured and constraint-based instructions

### 🔒 Deterministic Decoding
- Disabled randomness to improve stability

---

### 📊 Impact of Improvements

- More stable responses
- Reduced hallucination
- Better safety compliance

However, core model limitations still remain.

---

## 🧾 Conclusion

This project demonstrates how Large Language Models can be adapted into controlled and safety-aware systems using prompt engineering and simple rule-based filtering.

While the chatbot is capable of answering general health queries, it also highlights a key reality:

> **LLMs are powerful, but not inherently reliable for safety-critical applications.**

---

### 🧠 Key Takeaways

- Prompt engineering improves behavior but has limits  
- Model selection plays a critical role in performance  
- Safety requires multi-layer system design  
- Open-source models need additional alignment for sensitive domains  

---

This project reflects a practical understanding of building **responsible AI systems**, not just functional ones.

---

## 🚀 Future Work

This project can be significantly improved by:

- Fine-tuning the model on medical Q&A datasets  
- Using larger instruction-tuned models (e.g., Mistral, LLaMA)  
- Implementing Retrieval-Augmented Generation (RAG)  
- Adding ML-based safety classifiers  
- Integrating verified medical knowledge sources  

---

These improvements would make the system more reliable and production-ready.

---

## 🛠️ Tech Stack

- Python  
- HuggingFace Transformers  
- PyTorch  
- FLAN-T5  

---

## 👨‍💻 Author

**Muhammad Ali Waris Khan**  

---

## 📌 Note

This project is for educational purposes only and should not be used for real medical advice.
