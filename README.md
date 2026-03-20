# 🤖 AI Agent Lab

我的AI Agent学习实验室，从0到1构建智能体。

## 🎯 学习目标

- [x] 理解LLM基础与Prompt Engineering
- [x] 掌握Agent核心架构（ReAct、CoT等）
- [x] 实现工具调用（Tools/Function Calling）
- [x] 构建记忆系统（短期+长期）
- [x] 开发多Agent协作系统
- [x] 完成3个实战项目

## 📚 项目结构

```
ai-agent-lab/
├── 00-basics/              # 基础篇：LLM与Prompt基础
│   ├── 01-hello-llm/       # 初识大语言模型
│   ├── 02-prompt-101/      # Prompt工程入门
│   └── 03-structured-output/ # 结构化输出
│
├── 01-simple-agent/        # 简单Agent
│   ├── 01-reasoning/       # 推理能力（CoT、ReAct）
│   ├── 02-tool-use/        # 工具使用
│   └── 03-self-correction/ # 自我修正
│
├── 02-tools/               # 工具篇
│   ├── 01-web-search/      # 网络搜索工具
│   ├── 02-code-execution/  # 代码执行工具
│   └── 03-custom-tools/    # 自定义工具
│
├── 03-memory/              # 记忆系统
│   ├── 01-conversation-memory/ # 对话记忆
│   ├── 02-vector-store/    # 向量存储
│   └── 03-knowledge-base/  # 知识库构建
│
├── 04-multi-agent/         # 多Agent系统
│   ├── 01-agent-delegation/ # Agent委派
│   ├── 02-role-playing/    # 角色扮演
│   └── 03-workflow/        # 工作流编排
│
├── 05-projects/            # 实战项目
│   ├── 01-research-assistant/ # 研究助手
│   ├── 02-coding-agent/    # 编程助手
│   └── 03-data-analyst/    # 数据分析助手
│
├── shared/                 # 共享工具与配置
├── .env.example            # 环境变量模板
└── requirements.txt        # 依赖清单
```

## 🚀 快速开始

### 1. 安装依赖

```bash
pip install -r requirements.txt
```

### 2. 配置环境变量

```bash
cp .env.example .env
# 编辑 .env 填入你的 API 密钥
```

### 3. 开始学习

建议按目录顺序学习，每个模块包含完整的示例代码。

## 🛠️ 技术栈

| 类别 | 技术 |
|:---|:---|
| 编程语言 | Python 3.12+ |
| LLM API | OpenAI API / Anthropic Claude / 国产大模型 |
| 数据验证 | Pydantic v2 |
| 向量存储 | ChromaDB / Pinecone（可选） |
| 框架 | LangChain / LlamaIndex（可选） |
| 开发工具 | pytest, black |

## 📖 学习路径

| 阶段 | 目录 | 核心概念 | 状态 |
|:---|:---|:---|:---:|
| 1. 基础 | `00-basics/` | LLM调用、Prompt设计、结构化输出 | 📝 |
| 2. 入门 | `01-simple-agent/` | 推理链、工具调用、自我修正 | 📝 |
| 3. 工具 | `02-tools/` | 搜索、代码执行、自定义工具 | 📝 |
| 4. 记忆 | `03-memory/` | 对话历史、向量检索、知识库 | 📝 |
| 5. 多Agent | `04-multi-agent/` | Agent协作、角色定义、工作流 | 📝 |
| 6. 实战 | `05-projects/` | 完整应用开发 | 📝 |

> 📝 = 待完成 / 🚧 = 进行中 / ✅ = 已完成

## ⚙️ 环境配置说明

复制 `.env.example` 为 `.env`，配置以下变量：

```bash
# 必需：API 密钥
OPENAI_API_KEY=your-api-key-here

# 可选：自定义 Base URL（支持国产模型）
OPENAI_BASE_URL=https://api.openai.com/v1

# 可选：默认模型
DEFAULT_MODEL=gpt-3.5-turbo
```

支持多种模型提供商：
- OpenAI (GPT-4, GPT-3.5)
- 国产模型（Moonshot、DeepSeek、SiliconFlow等）
- Anthropic Claude

## 🤝 贡献

欢迎提交 Issue 和 PR 来完善这个学习项目！

## 📄 License

MIT License
