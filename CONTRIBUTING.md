# 贡献指南

感谢你愿意一起完善这份开源 LLM 应用开发学习路线。

这个项目希望保持一个清晰的定位：帮助开发者基于现有开源模型构建 LLM 应用，而不是从零训练基础模型。

## 可以贡献什么

欢迎贡献这些内容：

- 修正错别字、链接、表述不清的地方
- 补充某个阶段的学习资源
- 增加实践项目建议
- 补充 RAG、工具调用、微调、部署的经验
- 提供中文场景下的模型选择和评估经验
- 改进 HTML 页面结构或样式
- **分享你的学习成果和项目作品**

## 内容原则

请尽量遵循以下原则：

- 面向应用开发，不把重点放在大模型底层研究。
- 优先补充可实践、可验证、可复现的内容。
- 推荐工具时说明适用场景，而不是只堆名字。
- 不把某个框架描述成唯一选择。
- 区分“适合 RAG 的问题”和“适合微调的问题”。
- 对部署、安全、评估保持工程化视角。

## 提交 Pull Request

1. Fork 本仓库。
2. 创建你的分支。

```bash
git checkout -b improve-roadmap
```

3. 修改内容并提交。

```bash
git add .
git commit -m "Improve RAG learning section"
```

4. 推送到你的 Fork。

```bash
git push origin improve-roadmap
```

5. 在 GitHub 上创建 Pull Request。

## 页面编辑建议

当前项目是纯静态 HTML：

- 主页：`index.html`
- 通用样式：`styles.css`
- 每个阶段：独立文件夹下的 `index.html`

如果新增阶段，请同时更新：

- 根目录 `index.html`
- 相关阶段页面的上一阶段/下一阶段链接
- README 中的路线表格

## Issue 建议

提交 Issue 时，建议说明：

- 你想改进哪一部分
- 当前内容有什么问题
- 你建议如何修改
- 是否愿意提交 PR

## 学习作业提交指南

欢迎分享你在学习过程中完成的项目作品！

### 方式一：GitHub Discussions（推荐）

1. 在仓库的 [Discussions](https://github.com/reminder2021/open-llm-app-roadmap/discussions) 页面
2. 选择 **📣 Show and Tell** 频道
3. 创建新帖子，包含：
   - 项目名称和简要描述
   - 完成了哪个阶段的学习
   - 项目截图或 GIF
   - GitHub 仓库链接（如果开源）
   - 学习心得或踩坑记录

### 方式二：提交 Pull Request

如果你想让作品展示在 [作品展示页面](showcase/index.html)：

1. Fork 本仓库
2. 在 `showcase/projects/` 目录下创建你的项目页面
3. 参考 `showcase/index.html` 中的模板
4. 提交 Pull Request

### 作业展示要求

无论选择哪种方式，请确保：

- ✅ 有清晰的 README 说明如何运行
- ✅ 代码有基本的注释
- ✅ 不包含敏感信息（API Key、密码等）
- ✅ 说明完成了哪个阶段的学习任务
- ✅ 分享你的学习心得或踩坑记录（可选但推荐）

### 优秀作品标准

我们特别欢迎以下类型的项目：

- 完成了某个阶段的核心学习目标
- 有创新的实现方式或优化思路
- 包含详细的文档和注释
- 有实际的应用场景
- 分享了有价值的踩坑经验

谢谢你的贡献。
