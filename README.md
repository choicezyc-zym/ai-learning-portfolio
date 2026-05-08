# AI Learning Portfolio

This repository summarizes my AI learning journey and project portfolio.

The projects cover traditional machine learning, deep learning, Retrieval-Augmented Generation, AI Agent tool calling, and a combined RAG + Agent system.

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
        ↓
RAG + AI Agent
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

### 5. RAG Agent Project

**Type:** RAG + AI Agent  
**Tech Stack:** Python, Sentence Transformers, scikit-learn, Ollama, Qwen2.5, JSON Tool Calling

This project combines a local Retrieval-Augmented Generation system with an AI Agent.

The RAG pipeline is wrapped as a callable `rag_tool`, allowing the Agent to decide whether to use a calculator, read a local file, call the RAG tool, or use a general LLM response.

**Main Features:**

- Local knowledge base
- Text chunking
- Sentence embedding generation
- Cosine similarity semantic retrieval
- Dynamic chunk filtering
- RAG pipeline wrapped as a callable tool
- JSON-based tool call planning
- Python tool execution
- Calculator tool
- File reader tool
- General LLM response
- Agent execution history logging
- Lazy loading for the embedding model and RAG index

**Core Idea:**

```text
RAG is a knowledge tool.
Agent is the controller.
```

**Repository:**  
[rag-agent-project](https://github.com/choicezyc-zym/rag-agent-project)

---

## Technical Summary

Through these projects, I practiced:

- Traditional machine learning workflow
- Deep learning model training with PyTorch
- CNN image classification
- Semantic embedding and vector retrieval
- Retrieval-Augmented Generation
- Local LLM integration with Ollama
- Prompt construction
- Source citation
- JSONL logging
- AI Agent tool calling
- JSON-based tool call planning
- Python tool execution
- RAG tool wrapping
- Lazy loading optimization
- Project structuring and GitHub documentation

---

## Project List

| Project | Type | Main Technologies |
|---|---|---|
| student_pass_project | Traditional Machine Learning | Python, pandas, scikit-learn |
| mnist_cnn_project | Deep Learning / CNN | Python, PyTorch, MNIST |
| mini-rag-project | RAG | Python, Sentence Transformers, Ollama, Qwen2.5 |
| mini-agent-project | AI Agent | Python, Ollama, Qwen2.5, JSON tool calling |
| rag-agent-project | RAG + AI Agent | Python, Sentence Transformers, Ollama, Qwen2.5, JSON tool calling |

---

## Overall Reflection

These projects helped me understand the difference between different types of AI systems.

A traditional machine learning model learns patterns from structured data.

A CNN model learns visual features from image data.

A RAG system retrieves external knowledge before generating an answer.

An AI Agent can choose tools and execute tasks instead of only generating text.

A RAG Agent combines retrieval, tool calling, local LLM generation, and Python execution into one system.

The most important lesson is that modern AI applications are not just about calling a large language model. They usually combine models, data, retrieval, tools, logging, and engineering workflows.

---

## 中文项目总结

这个仓库记录了我的 AI 学习项目路线。

目前我完成了五个主要项目：

---

### 1. student_pass_project

这是一个传统机器学习项目，用于理解数据预处理、特征处理、模型训练和分类预测流程。

主要学习内容包括：

- 数据预处理
- 特征处理
- 训练集和测试集划分
- 模型训练
- 模型评估
- 传统机器学习完整流程

---

### 2. mnist_cnn_project

这是一个 PyTorch CNN 图像分类项目，用于理解深度学习训练流程、卷积神经网络结构和图像分类任务。

主要学习内容包括：

- PyTorch 训练流程
- Dataset 和 DataLoader
- CNN 网络结构
- 前向传播
- 损失函数
- 优化器
- 图像分类模型评估

---

### 3. mini_rag_project

这是一个本地 RAG 问答系统。

它基于本地 `knowledge.txt` 知识库进行语义检索，再调用本地 Qwen2.5 模型生成答案。

主要功能包括：

- 文本切块
- embedding 向量化
- cosine similarity 检索
- 动态相似度过滤
- 本地 LLM 生成答案
- 来源引用
- 多轮命令行问答
- JSONL 问答历史记录

核心思想是：

```text
先检索相关资料，再让大语言模型基于资料生成答案。
```

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

### 5. rag-agent-project

这是一个本地 RAG + AI Agent 结合项目。

它把 RAG 系统封装成 `rag_tool`，让 Agent 可以根据用户任务自动选择不同工具，包括计算器、文件读取、RAG 知识库问答和普通 LLM 回答。

主要功能包括：

- 本地知识库
- 文本切块
- embedding 向量化
- cosine similarity 语义检索
- 动态 chunk 过滤
- RAG 工具封装
- JSON 结构化工具调用
- calculator_tool 计算器工具
- file_reader_tool 文件读取工具
- 普通 LLM 问答
- embedding 模型和索引懒加载
- agent_history.jsonl 执行历史记录

核心思想是：

```text
RAG 是知识工具，Agent 是调度器。
```

---

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
    ↓
RAG + AI Agent
```

这条路线帮助我逐步理解现代 AI 应用的构建方式：

从基础预测模型，到神经网络，再到基于知识库的问答系统，然后到能够调用工具执行任务的 Agent 系统，最后把 RAG 和 Agent 结合，构建一个可以调用知识库工具的本地 AI 系统。

---

## Final Summary

This portfolio shows my step-by-step AI learning path.

I started from basic machine learning, then learned deep learning with CNNs, then built a local RAG system, then built a minimal AI Agent system, and finally combined RAG with Agent tool calling.

The main thing I learned is that AI applications are not only about models. A real AI system usually needs data processing, model inference, retrieval, tools, logging, and clear project structure.