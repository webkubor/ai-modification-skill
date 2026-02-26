---
name: ai-modification
description: Transform any project into an AI-native workspace. Manages llms.txt, llms-ctx.txt, and WebMCP discovery protocols.
version: 1.0.0
---

# 🤖 AI Modification Expert

本技能专注于将项目结构改造为“AI 原生”状态，确保大模型能以最高效率读取项目上下文。

## 🛠 核心能力

1. **LLMs.txt 自动化**:
   - 扫描 `docs/`, `rules/`, `skills/` 等目录。
   - 自动生成 `llms.txt` (全量) 和 `llms-ctx.txt` (精简)。
   - 提取 Markdown 标题作为描述。

2. **WebMCP 协议注入**:
   - 注入 `/.well-known/webmcp.json` 探测桩。
   - 建立 `window.mcp` 运行时接口规范。

## 📖 操作指南

### 当触发 "AI 改造" 时：
1. **询问决策**：必须向用户确认：“老爹，您是想进行 **llms.txt (文档索引化)** 还是 **WebMCP (接口自动化)** 改造？”
2. **执行 llms.txt**：调用 `node scripts/sync.js`。
3. **执行 WebMCP**：按照 WebMCP v2.0 规范，在项目根目录创建探测文件并注入接口。

## ⚙️ 工具调用参考
- **Sync**: `node scripts/sync.js`
