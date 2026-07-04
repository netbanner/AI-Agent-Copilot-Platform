# MVP（Minimum Viable Product）

Version: 1.0

Status: Draft

---

# Objective

第一版平台目标：

完成一个完整的 AI 使用闭环。

用户可以：

登录平台

↓

配置模型

↓

上传知识库

↓

开始聊天

↓

获得 AI 回复

↓

保存历史记录

整个流程能够完整运行。

---

# MVP Scope

包含以下模块：

## Identity

- 登录
- 注册
- JWT认证

---

## Workspace

- 默认 Workspace

---

## Dashboard

- 首页
- 最近聊天
- 最近知识库

---

## Models

支持：

- OpenAI
- DeepSeek
- Ollama（可选）

能够：

添加模型

编辑模型

测试连接

切换默认模型

---

## AI Chat

支持：

创建聊天

删除聊天

聊天历史

Streaming 输出

Markdown

代码高亮

上传文件

---

## Knowledge

支持：

创建知识库

上传 PDF

上传 Markdown

上传 TXT

文档解析

Chunk

Embedding

向量存储

Retriever

---

## Prompt Center

支持：

Prompt Template

变量

测试

---

# Not Included

以下功能不属于 MVP：

Workflow

Agent

Memory

Evaluation

Plugin

Marketplace

Billing

多租户

企业权限

MCP

Monitoring

---

# Success Criteria

满足以下条件：

✅ 用户能够登录

✅ 能够配置模型

✅ 能上传知识库

✅ 能完成 Embedding

✅ 能聊天

✅ AI 能引用知识库回答

✅ 能保存聊天记录

即可发布：

v0.1

---

# Technical Goal

完成：

Spring Boot

Spring AI

PostgreSQL

Redis

pgvector

Next.js

Docker

完整集成

---

# Deliverables

Backend

Frontend

Database

API

Deployment

Documentation

全部完成。

---

# Next Step

下一阶段：

Feature List

开始拆解每个模块。
