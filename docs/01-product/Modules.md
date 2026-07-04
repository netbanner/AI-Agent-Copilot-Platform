# Modules

Version: 1.0

---

# Overview

AI Agent & Copilot Platform

由多个独立业务模块组成。

每个模块拥有自己的业务职责。

模块之间通过接口进行通信。

---

# Module 1

Identity

## Responsibility

负责用户认证。

负责授权。

负责登录。

负责Token。

负责API Key。

### Includes

- Login
- Register
- JWT
- OAuth
- Session

---

# Module 2

Workspace

## Responsibility

负责工作空间。

团队。

成员。

角色。

权限。

### Includes

- Workspace
- Member
- Team
- Role
- Permission

---

# Module 3

Dashboard

## Responsibility

系统首页。

数据统计。

最近访问。

系统状态。

### Includes

- Dashboard
- Statistics
- Recent Chat
- Recent Knowledge
- Usage

---

# Module 4

Models

## Responsibility

统一模型管理。

### Includes

- OpenAI
- Gemini
- Claude
- DeepSeek
- Ollama
- Router
- Cost

---

# Module 5

Chat

## Responsibility

AI 对话。

Copilot。

上下文管理。

聊天历史。

### Includes

- Conversation
- Message
- Streaming
- Markdown
- Upload
- History

---

# Module 6

Knowledge

## Responsibility

企业知识库。

RAG。

文档管理。

### Includes

- Knowledge Base
- Documents
- Upload
- Chunk
- Embedding
- Retriever
- Search

---

# Module 7

Prompt

## Responsibility

Prompt 管理。

模板。

版本。

变量。

### Includes

- Prompt
- Template
- Version
- Variable

---

# Module 8

Workflow

## Responsibility

AI Workflow。

流程设计。

节点执行。

### Includes

- Workflow
- Node
- Edge
- Variables
- Execution

---

# Module 9

Agents

## Responsibility

AI Agent。

规划。

记忆。

工具。

### Includes

- Agent
- Memory
- Planning
- Tasks
- Evaluation

---

# Module 10

Tools

## Responsibility

Tool Calling。

MCP。

第三方系统。

### Includes

- Browser
- GitHub
- Database
- HTTP
- MCP

---

# Module 11

Files

## Responsibility

统一文件中心。

### Includes

- Upload
- Images
- PDFs
- Storage
- Preview

---

# Module 12

Administration

## Responsibility

后台管理。

日志。

配置。

### Includes

- User
- Role
- Logs
- Config
- Audit

---

# Dependency

Identity

↓

Workspace

↓

Dashboard

↓

Models

↓

Chat

↓

Knowledge

↓

Prompt

↓

Workflow

↓

Agents

↓

Tools

↓

Administration
