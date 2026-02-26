# 🤖 AI Modification Expert (Gemini Skill)

[![Gemini CLI](https://img.shields.io/badge/Gemini--CLI-Skill-blueviolet)](https://github.com/google-gemini/gemini-cli)
[![Status](https://img.shields.io/badge/Status-Beta-orange)](https://github.com/webkubor)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**AI Modification Expert** 是一个为 [Gemini CLI](https://github.com/google-gemini/gemini-cli) 打造的自动化“AI 原生化”改造工具。它旨在将任何项目转化为对 AI 极其友好的架构，大幅提升 AI Agent 的上下文理解准确度和响应速度。

## ✨ 核心特性

- **📄 LLMs.txt 自动化**：一键生成符合行业最新标准的 `llms.txt` 和 `llms-ctx.txt` 索引。
- **🔌 WebMCP 注入**：内置 WebMCP 协议（Model Context Protocol）注入逻辑，为网页提供标准化的 AI 接口。
- **🧹 文档脱敏与精简**：自动提取 Markdown 标题，消除冗余 HTML 噪音，为 AI 提供“高纯度”喂料。
- **🔄 动态同步**：支持后台主进程静默更新索引，确保 AI 永远掌握最新地图。

## 🛠 安装指南

确保您已安装 [Gemini CLI](https://github.com/google-gemini/gemini-cli)，然后在终端执行：

```bash
gemini skills install https://raw.githubusercontent.com/webkubor/gemini-skill-ai-native/main/ai-modification.skill --scope user
```

## 📖 使用方法

您可以对 Gemini 发出以下指令：

- *"进行 AI 改造"* (会提示您选择 `llms.txt` 还是 `webmcp`)
- *"帮我生成 llms.txt"*
- *"给网站加个 WebMCP 接口"*

## ⚙️ 目录结构

符合 Anthropic Skills 与 Gemini CLI 混合规范：
- `SKILL.md`: 技能大脑指令（Instructions）。
- `scripts/sync.js`: 核心同步逻辑脚本。
- `LICENSE`: MIT 协议。

---
Created by [webkubor](https://github.com/webkubor)
"AI Native Architecture" - Made with ❤️ by Candle.
