# 🚀 Multi-Agent Finance AI System (LangGraph + MCP + RAG)
## 项目结构
multi-agent-finance-ai/
├── README.md
├── backend/
│   ├── main.py
│   ├── config.py
│   │
│   ├── graph/
│   │   └── agent_graph.py
│   │
│   ├── agents/
│   │   ├── planner.py
│   │   ├── advisor.py
│   │   ├── research.py
│   │
│   ├── tools/
│   │   └── fund_tools.py
│   │
│   ├── rag/
│   │   ├── vector_store.py
│   │   └── retriever.py
│   │
│   ├── memory/
│   │   └── memory_store.py
│   │
│   ├── reflection/
│   │   └── reflector.py
│   │
│   ├── eval/
│   │   └── evaluator.py
│   │
│   └── utils/
│       └── llm.py
│
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   └── ChatBox.jsx
│
└── requirements.txt

## 📌 项目简介

本项目实现了一套基于 **LangGraph 的多Agent AI系统**，模拟智能投顾场景，通过引入：

* 多Agent协同（Planner / Research / Advisor）
* MCP风格Tool调用
* RAG知识增强
* Memory用户长期记忆
* Reflection自反思机制

构建了一个具备“感知-决策-执行-评估”闭环的AI应用系统。

---

## 🧠 系统架构

用户输入 → Memory → 多轮对话 → Planner → Agent执行 → Tool调用 / RAG → Reflection → 输出结果

---

## ⚙️ 技术栈

* Backend: FastAPI + LangGraph
* LLM: OpenAI / DeepSeek
* RAG: FAISS + Embedding
* Frontend: React
* 架构: Multi-Agent + MCP Tool

---

## ✨ 核心能力

### 1️⃣ 多Agent调度

基于LangGraph实现Agent编排，支持任务拆解与动态路由。

### 2️⃣ MCP Tool调用

将金融能力封装为工具接口，实现LLM与结构化能力解耦。

### 3️⃣ RAG知识增强

通过向量数据库实现知识检索，提高回答准确性。

### 4️⃣ Memory（长期记忆）

记录用户风险偏好，实现个性化推荐。

### 5️⃣ Reflection（自反思）

自动评估结果质量，并在必要时重试优化。

---

## 📦 快速启动

```bash
pip install -r requirements.txt
uvicorn backend.main:app --reload
```

前端：

```bash
cd frontend
npm install
npm start
```

---

## 🧪 示例问题
* 帮我分析某只基金收益
* 我是低风险用户，帮我做资产配置
* 最近市场怎么样

---

## 📊 项目亮点
* 完整AI Agent系统闭环（Memory + Reflection）
* 类盈米MCP架构（能力工具化）
* 支持多轮对话与个性化推荐
* 可扩展至任意行业AI系统

---

## 📈 后续优化方向
* 引入LangGraph Memory模块
* 接入真实金融数据API
* 增加Agent自学习能力

---

## 📬 作者
hesm
