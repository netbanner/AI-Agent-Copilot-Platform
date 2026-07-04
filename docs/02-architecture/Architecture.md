# Architecture Overview

Project

AI Agent & Copilot Platform

Version

1.0

Status

Draft

---

# 1. Architecture Goal

构建一个：

模块化

可扩展

企业级

AI Native

平台。

平台支持：

Chat

Knowledge

Agent

Workflow

Multi LLM

Tool Calling

RAG

未来支持：

企业部署

多租户

插件系统

---

# 2. Architecture Principles

整个系统遵循以下原则：

## Modular Monolith First

第一阶段：

采用：

模块化单体。

不是：

微服务。

原因：

降低复杂度。

提高开发效率。

方便重构。

未来：

可以逐步拆分。

---

## API First

所有能力：

优先设计 API。

UI 只是 API Consumer。

---

## Domain Driven Design

按业务领域划分模块。

不是：

Controller。

不是：

数据库。

例如：

Chat

Knowledge

Workflow

Agent

---

## AI Native

AI

不是：

插件。

而是：

平台核心。

所有模块围绕 AI。

---

## Event Driven

模块之间：

尽量事件通信。

降低耦合。

---

## Cloud Native Ready

未来支持：

Docker

Kubernetes

CI/CD

Horizontal Scaling

---

# 3. High Level Architecture

整个系统：

```

                    Browser
                        │
         ┌──────────────┴──────────────┐
         │                             │
      Next.js Frontend            Admin UI
         │
         ▼
      Spring Boot API
         │
 ┌───────┼──────────────────────────────────────────┐
 │       │          │          │         │          │
 ▼       ▼          ▼          ▼         ▼          ▼
Chat  Knowledge  Workflow   Agent    Models     Files
 │       │          │          │         │
 └───────┴──────────┴──────────┴─────────┘
                    │
              Platform Core
                    │
        ┌───────────┼────────────┐
        ▼           ▼            ▼
   PostgreSQL     Redis      Object Storage

```

---

# 4. Layered Architecture

系统采用四层架构。

Presentation Layer

↓

Application Layer

↓

Domain Layer

↓

Infrastructure Layer

职责：

Presentation

负责：

HTTP

REST

SSE

WebSocket

Application

负责：

Use Case

业务流程

Domain

负责：

业务规则

Infrastructure

负责：

数据库

Redis

LLM

对象存储

第三方接口

---

# 5. Core Modules

Identity

Workspace

Dashboard

Chat

Knowledge

Prompt

Workflow

Agent

Models

Tools

Files

Administration

Platform

---

# 6. Future Evolution

MVP

↓

Modular Monolith

↓

Module Extraction

↓

Microservices（如需要）

↓

Cloud Native

↓

Enterprise Platform

---

# 7. Why Modular Monolith

为什么不是微服务？

因为：

当前：

只有一个团队。

业务快速变化。

架构频繁调整。

模块化单体：

更容易：

重构。

调试。

测试。

未来：

成熟后：

再拆微服务。

---

# Next Step

Tech Stack

