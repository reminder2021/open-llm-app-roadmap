# 开源 LLM 应用开发学习路线

这是一个面向 **LLM 应用开发工程师** 的学习路线项目。

目标不是从零训练或开发一个大模型，而是基于现有开源模型，学习如何构建真正可用的 LLM 应用，包括：

- 开源模型选择与本地推理
- Prompt 与结构化输出
- RAG 知识库问答
- Tool Calling / Function Calling
- LangChain 与 LangGraph 应用编排
- LoRA / QLoRA 微调
- 评估体系
- 部署与工程化

在线浏览时，可以直接打开项目中的 `index.html`。

## 项目定位

很多 LLM 学习资料会从 Transformer、预训练、模型结构开始讲起。那些内容很重要，但并不一定是应用开发者的第一优先级。

这个项目更关注：

- 如何把开源模型跑起来
- 如何让模型接入自己的数据
- 如何让模型调用工具
- 如何判断什么时候该用 RAG，什么时候该微调
- 如何把 Demo 变成可部署、可评估、可维护的系统

适合人群：

- 想学习 LLM 应用开发的程序员
- 想基于开源模型做知识库、助手、Agent 的开发者
- 已经会一点 Python，希望进入 AI 应用方向的人
- 不打算从零训练大模型，但希望掌握微调和部署的人

## 学习路线

项目按阶段拆分为独立页面：

| 阶段 | 内容 |
| --- | --- |
| 00 | 总览与学习方式 |
| 01 | Python 与 Web API 基础 |
| 02 | 开源模型使用与推理服务 |
| 03 | Prompt 与结构化输出 |
| 04 | RAG 知识库问答 |
| 05 | 工具调用、LangChain 与 LangGraph |
| 06 | LoRA/QLoRA 微调 |
| 07 | 评估体系 |
| 08 | 部署与工程化 |
| 09 | 综合项目作品集 |

## 推荐学习顺序

```text
Python / Web API 基础
→ 开源模型推理
→ Prompt 与结构化输出
→ RAG
→ 手写 Tool Calling
→ LangChain / LangGraph
→ LoRA / QLoRA 微调
→ 评估体系
→ 部署与工程化
→ 综合项目
```

其中 LangChain 和 LangGraph 的建议学习方式是：

```text
先理解底层机制，再使用框架提高效率。
```

也就是说，建议先手写一遍基础 RAG 和工具调用，再学习 LangChain 的组件抽象和 LangGraph 的状态编排。

## 如何本地查看

方式一：直接打开 HTML 文件。

```text
open-llm-app-roadmap/index.html
```

方式二：启动一个简单本地服务器。

```bash
python3 -m http.server 8000
```

然后在浏览器访问：

```text
http://localhost:8000
```

## 如何发布到 GitHub Pages

1. 在 GitHub 创建仓库，仓库名建议为：

```text
open-llm-app-roadmap
```

2. 将本项目推送到 GitHub。

```bash
git init
git add .
git commit -m "Initial roadmap site"
git branch -M main
git remote add origin https://github.com/<your-username>/open-llm-app-roadmap.git
git push -u origin main
```

请把 `<your-username>` 替换成你的 GitHub 用户名。

3. 打开 GitHub 仓库页面：

```text
Settings → Pages
```

4. 在 `Build and deployment` 中选择：

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

5. 保存后等待 GitHub Pages 构建完成。

发布后的地址通常是：

```text
https://<your-username>.github.io/open-llm-app-roadmap/
```

## 仓库结构

```text
open-llm-app-roadmap/
├── index.html
├── styles.css
├── 00-overview/
├── 01-foundations/
├── 02-open-source-models/
├── 03-prompt-structured-output/
├── 04-rag/
├── 05-tool-calling-langchain-langgraph/
├── 06-finetuning/
├── 07-evaluation/
├── 08-deployment/
├── 09-capstone-projects/
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```

## 贡献

欢迎提交 Issue 或 Pull Request，尤其欢迎补充：

- 更好的学习资料
- 实战项目案例
- 中文开源模型实践经验
- RAG、Agent、微调、部署踩坑记录
- 路线结构优化建议

贡献前可以先阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。

## License

本项目使用 [MIT License](LICENSE)。
