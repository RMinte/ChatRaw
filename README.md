<div align="center">

# ChatRaw 🚀

**Minimalist AI Chat Interface | 极简 AI 聊天界面**

*30s deployment, zero registration, any OpenAI-compatible API*

*30秒部署，零注册，支持任意 OpenAI 兼容 API*

![License](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-blue.svg)
![Python](https://img.shields.io/badge/Python-3.12+-3776AB?logo=python)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?logo=docker)

</div>

---

<details open>
<summary><b>🇺🇸 English</b></summary>

## 💡 Why ChatRaw?

Existing open-source chat frontends are too heavy and complex. Many developers and AI hardware vendors simply need a clean, ready-to-use, minimal chat tool that supports any OpenAI-compatible API, allows drag-and-drop document RAG, requires zero registration, and can be deployed with one click — to demo their AI hardware or local models to clients in 30 seconds.

**ChatRaw was born for this.**

## ✨ Features

- 🪶 **Ultra Lightweight** - Single binary, ~15MB Docker image
- ⚡ **Instant Startup** - Millisecond launch, <20MB memory
- 🔌 **Plug & Play** - Any OpenAI-compatible API (Ollama, vLLM, LocalAI, etc.)
- 📄 **Drag & Drop RAG** - Upload documents for instant Q&A
- 🖼️ **Vision AI** - Multimodal image understanding
- 🌍 **i18n** - English & Chinese with one-click switch
- 🔒 **Zero Registration** - Settings auto-saved locally
- 🐳 **One-Click Deploy** - Docker Compose in 30 seconds

## 🚀 Quick Start

**Option 1: One Command**
```bash
docker run -d -p 51111:51111 -v chatraw_data:/app/data --name chatraw massif01/chatraw:latest
```

**Option 2: Git Clone**
```bash
git clone https://github.com/massif-01/ChatRaw.git
cd ChatRaw
docker compose up -d
```

**Visit http://localhost:51111**

## ⚙️ Configuration

### Models

| Type | Description | Examples |
|------|-------------|----------|
| Chat | Chat model | llama3.2, qwen2.5, gpt-4 |
| Embedding | Vector model | nomic-embed-text, bge-large |
| Reranker | Rerank model | bge-reranker |

### Chat Settings

| Parameter | Default |
|-----------|---------|
| Temperature | 0.7 |
| Top P | 0.9 |
| Stream | true |

### RAG Settings

| Parameter | Default |
|-----------|---------|
| Chunk Size | 500 |
| Chunk Overlap | 50 |
| Top K | 3 |
| Score Threshold | 0.5 |

## 📝 API Compatibility

| Service | URL Example |
|---------|-------------|
| Ollama | `http://localhost:11434/v1` |
| vLLM | `http://localhost:8000/v1` |
| LocalAI | `http://localhost:8080/v1` |
| LM Studio | `http://localhost:1234/v1` |
| OpenAI | `https://api.openai.com/v1` |

## 🔧 Environment Variables

| Variable | Default |
|----------|---------|
| PORT | 51111 |
| DATA_DIR | ./data |

</details>

---

<details>
<summary><b>🇨🇳 中文</b></summary>

## 💡 为什么选择 ChatRaw？

现有的开源聊天前端都太重太复杂了。很多开发者和 AI 硬件厂商其实只需要一个干净、开箱即用、支持任意 OpenAI 兼容 API、还能随便拖个文档就 RAG、零注册、一键部署的极简聊天工具，30秒给客户展示你的 AI 硬件/本地模型。

**ChatRaw 就是为此而生。**

## ✨ 特性

- 🪶 **极致轻量** - 单文件二进制，~15MB Docker 镜像
- ⚡ **极速启动** - 毫秒级启动，内存占用 <20MB
- 🔌 **即插即用** - 支持任意 OpenAI 兼容 API（Ollama、vLLM、LocalAI 等）
- 📄 **拖拽 RAG** - 拖个文档进来就能问答
- 🖼️ **视觉理解** - 支持多模态模型图片理解
- 🌍 **多语言** - 中英文一键切换
- 🔒 **零注册** - 无需登录，设置自动保存到本地
- 🐳 **一键部署** - Docker Compose 30秒部署

## 🚀 快速开始

**方式一：一行命令**
```bash
docker run -d -p 51111:51111 -v chatraw_data:/app/data --name chatraw massif01/chatraw:latest
```

**方式二：克隆仓库**
```bash
git clone https://github.com/massif-01/ChatRaw.git
cd ChatRaw
docker compose up -d
```

**访问 http://localhost:51111**

## ⚙️ 配置说明

### 模型类型

| 类型 | 说明 | 示例 |
|------|------|------|
| 聊天 | 聊天模型 | llama3.2, qwen2.5, gpt-4 |
| 嵌入 | 向量模型 | nomic-embed-text, bge-large |
| 重排 | 重排序模型 | bge-reranker |

### 聊天设置

| 参数 | 默认值 |
|------|--------|
| 温度 | 0.7 |
| Top P | 0.9 |
| 流式输出 | 开启 |

### RAG 设置

| 参数 | 默认值 |
|------|--------|
| 文档块大小 | 500 |
| 块重叠 | 50 |
| Top K | 3 |
| 相似度阈值 | 0.5 |

## 📝 API 兼容性

| 服务 | URL 示例 |
|------|----------|
| Ollama | `http://localhost:11434/v1` |
| vLLM | `http://localhost:8000/v1` |
| LocalAI | `http://localhost:8080/v1` |
| LM Studio | `http://localhost:1234/v1` |
| OpenAI | `https://api.openai.com/v1` |

## 🔧 环境变量

| 变量 | 默认值 |
|------|--------|
| PORT | 51111 |
| DATA_DIR | ./data |

</details>

---

## 📄 License

This project is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

- ✅ Free for personal and non-commercial use
- ✅ Must give appropriate credit  
- ❌ Commercial use requires explicit permission
- ❌ Cannot remove copyright notices

Copyright © 2025 massif-01, RMinte AI Technology Co., Ltd.

See [LICENSE](LICENSE) for details.

---

<div align="center">

**ChatRaw** - Making AI Chat Simple Again

</div>
