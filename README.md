# Bright-Data-LangChain
Bright Data + LangChain 高效采集方案：7 分钟搭建实时数据管道


```markdown
# Bright Data + LangChain：7 分钟实时数据管道 🚀



不用写爬虫、不用处理反爬、不用解析 HTML。
这是一个**极简可落地**的方案，通过 Bright Data + LangChain + OpenAI，实现从网页采集到 AI 分析的全流程自动化。

## ✨ 核心亮点

1. **🚫 免开发爬虫**：Bright Data 自带 LinkedIn/Amazon/Google 等预定义模板，直接获取结构化 JSON。
2. **⚡ 极速集成**：7 分钟搭建 `采集 -> 分析 -> 输出` 的端到端管道。
3. **🤖 AI 智能驱动**：无缝对接大模型，轻松实现内容总结、数据评估、舆情分析。
4. **📁 标准输出**：结果导出为 JSON，完美接入数据库/BI/后端系统。

## 🏗️ 架构流程图

```mermaid
flowchart LR
    A[目标网页<br/>(LinkedIn/电商等)] --> B(Bright Data<br/>结构化采集)
    B --> C(LangChain<br/>数据调度)
    C --> D(OpenAI GPT<br/>智能分析)
    D --> E[analysis.json<br/>分析结果]
```

## 🚀 快速开始

### 1. 安装依赖

```bash
pip install python-dotenv langchain-brightdata langchain-openai requests
```

### 2. 配置环境变量

复制 `.env.example` 为 `.env` 并填入你的 API Key：

```env
BRIGHT_DATA_API_KEY="你的 Bright Data API Key"
OPENAI_API_KEY="你的 OpenAI API Key"
```

### 3. 运行脚本

```bash
python script.py
```

程序会自动采集指定网页数据，并调用 AI 生成分析报告，最终结果保存在 `analysis.json` 中。

## 📝 示例功能

- **采集目标**：LinkedIn 个人主页
- **AI 任务**：评估候选人是否适合远程软件工程师岗位
- **输出结果**：结构化的候选人资料 + AI 适配度评估

## 📄 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件
```

### 如何使用：
1. 直接复制上述代码，保存为你的项目根目录下的 `README.md`。
2. 修改其中的 `script.py` 引用说明和配置步骤即可。

这个版本既保留了专业度，又显得非常清爽，非常适合在 GitHub 上展示！
