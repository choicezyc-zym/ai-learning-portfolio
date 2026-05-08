# AI Learning Portfolio

This repository summarizes my AI learning journey and project portfolio.

The projects cover traditional machine learning, deep learning, retrieval-augmented generation, and AI Agent development.

---

## Learning Path

My learning path follows this order:

```text
Traditional Machine Learning
        ↓
Deep Learning
        ↓
Retrieval-Augmented Generation
        ↓
AI Agent
```

The goal is to gradually understand how modern AI systems are built, from basic prediction models to local LLM-based applications.

---

## Projects

### 1. Student Pass Prediction Project

**Type:** Traditional Machine Learning  
**Tech Stack:** Python, pandas, scikit-learn, machine learning models

This project is a traditional machine learning classification project.

It predicts whether a student may pass based on structured student-related data.

**Main Learning Points:**

- Data preprocessing
- Feature handling
- Train-test split
- Model training
- Model evaluation
- Basic machine learning workflow

**Repository:**  
[student_pass_project](https://github.com/choicezyc-zym/student_pass_project)

---

### 2. MNIST CNN Project

**Type:** Deep Learning / Computer Vision  
**Tech Stack:** Python, PyTorch, CNN, MNIST

This project uses a Convolutional Neural Network to classify handwritten digits from the MNIST dataset.

**Main Learning Points:**

- PyTorch training workflow
- Dataset and DataLoader
- CNN architecture
- Forward propagation
- Loss function and optimizer
- Model evaluation on image data

**Repository:**  
[mnist_cnn_project](https://github.com/choicezyc-zym/mnist_cnn_project)

---

### 3. Mini RAG Project

**Type:** Retrieval-Augmented Generation  
**Tech Stack:** Python, Sentence Transformers, cosine similarity, Ollama, Qwen2.5

This project is a minimal local RAG question-answering system.

It answers user questions based on a local knowledge file. The system first retrieves relevant text chunks from the local knowledge base, then sends the retrieved context to a local Qwen2.5 model through Ollama to generate grounded answers.

**Main Features:**

- Local knowledge base
- Text chunking
- Sentence embeddings
- Cosine similarity retrieval
- Dynamic similarity filtering
- Local LLM answer generation
- Source citation
- Multi-turn command-line interaction
- JSONL query history logging

**Core Idea:**

```text
Retrieve relevant context first, then generate an answer based on that context.
```

**Repository:**  
[mini-rag-project](https://github.com/choicezyc-zym/mini-rag-project)

---

### 4. Mini Agent Project

**Type:** Local AI Agent  
**Tech Stack:** Python, Ollama, Qwen2.5, JSON tool calling

This project is a minimal local AI Agent system.

It uses Qwen2.5 to generate a structured JSON tool call plan. Python then parses the plan and executes the selected tool.

**Supported Tools:**

- Calculator tool
- Local text file reader tool
- General LLM question-answering tool

**Main Features:**

- Local LLM integration
- JSON-based tool call planning
- Python tool execution
- Calculator tool
- File reader tool
- Multi-turn command-line interaction
- Agent execution history logging

**Core Idea:**

```text
LLM plans, Python executes.
```

**Repository:**  
[mini-agent-project](https://github.com/choicezyc-zym/mini-agent-project)

---




### 4. mini_agent_project


这是一个本地 AI Agent 项目。

它使用 Qwen2.5 生成 JSON 工具调用计划，再由 Python 调用计算器、文件读取或 LLM 工具完成任务。

主要功能包括：

- Qwen2.5 本地模型调用
- JSON 结构化工具调用
- calculator_tool 计算器工具
- file_reader_tool 文件读取工具
- 普通 LLM 问答工具
- 多轮命令行交互
- agent_history.jsonl 执行历史记录

核心思想是：

```text
LLM 负责规划，Python 负责执行。
```

---
### 5. RAG Agent Project

**Type:** RAG + AI Agent  
**Tech Stack:** Python, Sentence Transformers, Ollama, Qwen2.5, JSON Tool Calling

This project combines a local RAG system with an AI Agent.

It wraps the RAG pipeline as a callable `rag_tool`, allowing the Agent to decide whether to use calculator, file reader, RAG, or general LLM response based on the user task.

**Main Features:**

- Local knowledge base
- Semantic retrieval with Sentence Transformers
- Cosine similarity chunk retrieval
- RAG tool wrapping
- JSON-based tool call planning
- Python tool execution
- Calculator tool
- File reader tool
- General LLM response
- Agent execution history logging

**Core Idea:**

```text
RAG is a knowledge tool.
Agent is the controller.
## Learning Roadmap

整体学习路线是：

```text
传统机器学习
    ↓
深度学习
    ↓
RAG
    ↓
AI Agent
```

这条路线帮助我逐步理解现代 AI 应用的构建方式：

从基础预测模型，到神经网络，再到基于知识库的问答系统，最后到能够调用工具执行任务的 Agent 系统。

---

## Project List

| Project | Type | Main Technologies |
|---|---|---|
| student_pass_project | Traditional Machine Learning | Python, pandas, scikit-learn |
| mnist_cnn_project | Deep Learning / CNN | Python, PyTorch, MNIST |
| mini_rag_project | RAG | Python, Sentence Transformers, Ollama, Qwen2.5 |
| mini_agent_project | AI Agent | Python, Ollama, Qwen2.5, JSON tool calling |
| rag-agent-project | RAG + AI Agent | Python, Sentence Transformers, Ollama, Qwen2.5, JSON tool calling |

---

## Final Summary

This portfolio shows my step-by-step AI learning path.

I started from basic machine learning, then learned deep learning with CNNs, then built a local RAG system, and finally built a minimal AI Agent system.

The main thing I learned is that AI applications are not only about models. A real AI system usually needs data processing, model inference, retrieval, tools, logging, and clear project structure.