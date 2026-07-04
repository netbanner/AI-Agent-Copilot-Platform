# AI Agent & Copilot Platform

Version: 1.0

Status: Draft

Last Updated: 2026-07-03

---

# Product Map

AI Agent & Copilot Platform 是一个企业级 AI 应用开发平台。

平台主要由多个核心业务模块组成。

每一个模块未来都可以独立演进。

```
AI Agent & Copilot Platform
│
├── Workspace
├── Dashboard
├── AI Chat
├── Knowledge
├── Agents
├── Workflow
├── Models
├── Tools
├── Prompt Center
├── Files
├── Administration
└── Settings
```

---

# Module Overview

| Module | Description |
|----------|-------------|
| Workspace | 工作空间、团队、权限管理 |
| Dashboard | 首页、统计信息、最近使用内容 |
| AI Chat | AI 对话、Copilot、聊天记录 |
| Knowledge | 知识库、文档管理、RAG |
| Agents | AI Agent 创建与管理 |
| Workflow | AI 工作流设计与执行 |
| Models | 大模型管理与路由 |
| Tools | Tool Calling 与 MCP |
| Prompt Center | Prompt 模板与版本管理 |
| Files | 文件上传与统一存储 |
| Administration | 用户、角色、系统管理 |
| Settings | 系统配置与个人设置 |

---

# Module Relationship

Workspace

↓

所有业务均运行于 Workspace。

↓

Workspace

├── Dashboard
├── AI Chat
├── Knowledge
├── Agents
├── Workflow
├── Prompt Center
├── Models
├── Tools
├── Files
└── Settings

Administration

负责整个系统管理。

---

# Product Principles

平台遵循以下设计原则：

1. 模块化（Modular）

每个模块可以独立开发。

---

2. 可扩展（Extensible）

方便未来增加新的能力。

例如：

新的模型

新的 Agent

新的 Tool

新的 Workflow Node

---

3. 企业级（Enterprise Ready）

支持：

Workspace

Role

Permission

Audit

Monitoring

Deployment

---

4. AI Native

AI 是平台核心能力。

不是附加功能。

所有模块都围绕 AI 展开。

---

5. API First

所有能力优先提供 API。

UI 只是 API 的消费者。

---

6. Documentation First

每个模块：

先完成设计文档。

再开始编码。

---

# Current Scope

当前版本（MVP）重点开发：

✅ Authentication

✅ Dashboard

✅ AI Chat

✅ Knowledge

✅ Models

✅ Prompt Center

后续版本：

Workflow

↓

Agent

↓

Tools

↓

Enterprise

---

# Out of Scope

当前阶段：

不开发：

Billing

Marketplace

Mobile

Multi-region

SaaS

复杂企业 IAM

未来版本再逐步加入。

---

# Next Document

完成 Product Map 后，

下一步：

MVP.md

定义：

第一版真正开发哪些模块。
