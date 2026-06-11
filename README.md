<div align="center">

# 出处 · Provenance

**溯源 · 金句化 · 引用库**

一句话找到真实出处，或将你的意思改写成金句表达。

单文件 HTML · 零依赖 · 零后端 · 数据本地存储

[立即使用](https://chuchu.gzl406633204.workers.dev) · [功能介绍](#-功能)  · [English](#english)

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML](https://img.shields.io/badge/built%20with-HTML%2FJS-orange.svg)
![DeepSeek](https://img.shields.io/badge/powered%20by-DeepSeek-green.svg)

</div>

---

## 这是什么

你有没有过这样的情况——隐约记得某本书或电影里有句让你印象深刻的话，但说不出准确的原文与出处，只能含糊地说"我记得哪里好像说过……"

**出处** 就是为解决这个问题而生的工具。输入你记得的大意，它会找到真实存在的原文、作品、作者，以及置信度评级。你还可以输入自己想表达的意思，让它为你匹配真实的名家引用，或将你的话改写为金句质感的表达。

所有功能运行在单一 HTML 文件内，浏览器打开即用，无需安装，无需账号，数据完全保存在本机。

---

## ✨ 功能

### 🔍 溯源
输入模糊记忆中的话（不必是原文，大意即可）→ 返回：

| 字段 | 说明 |
|---|---|
| 原文 | 通行中文原文，外文著作同步给出原句 |
| 出处 | 作品名、作者、年份、章节/场景 |
| 置信度 | 高 / 中（建议核实）/ 低（不建议引用）|
| 讹传警示 | 许多流行"名言"实为误归，工具明确提示 |
| 候选出处 | 折叠展示其他可能的来源 |

> 找不到时诚实告知，**绝不编造出处**。

---

### ✍️ 金句化
输入你想表达的意思，选择场景与语气 → 返回两个严格分区的结果：

**A · 真实名家引用**（可注明出处）
- 确实存在的金句，附出处与置信度
- 仅展示高/中置信度结果，宁缺毋滥

**B · 原创改写**（以你自己的名义说）
- 将你的意思改写为 3 条金句质感表达
- 明确标注为原创，绝不伪造来源

| 场景 | 语气 |
|---|---|
| 日常交谈 / 演讲发言 / 文章写作 / 社交媒体 | 哲思 / 温暖 / 犀利 / 幽默 |

---

### 📚 引用库
- 一键收藏溯源与金句化的结果
- 真实引用与原创改写分类存储
- 关键词搜索、删除管理
- **JSON 导出 / 导入**，方便多设备迁移

---

## 🛠 技术说明

```
架构   单文件 HTML + 原生 JavaScript，无构建步骤，无外部依赖
AI     DeepSeek Chat Completions API（deepseek-chat / deepseek-reasoner 可选）
存储   API Key 与引用库均保存于本机 localStorage，无后端，无数据上传
设计   Apple 设计语言——系统字体、浅灰底色、毛玻璃导航、单一蓝色点缀
响应式 桌面/移动端自适应，支持 iOS 安全区与 prefers-reduced-motion
```

---

## 🛡 防幻觉机制

AI 溯源存在固有的幻觉风险，本工具通过多层机制降低误差：

1. **Prompt 铁律**：系统提示词明确"宁可回答找不到，严禁编造出处"
2. **强制置信度**：每条结果自评置信度，低置信结果独立警示且不建议引用
3. **讹传检测**：误归于名人的"伪名言"单独标注说明
4. **金句化双轨制**：真实引用与原创改写严格分区，视觉上绝不混淆

**注意**：AI 对冷门著作和台词细节的准确率有限。重要场合引用前，请自行核实原文。

---

## 🔒 隐私

- 无数据采集，无统计埋点，无 Cookie
- 你的输入仅发送至 DeepSeek API 用于生成结果，遵循 [DeepSeek 隐私政策](https://www.deepseek.com/privacy)
- API Key 仅存储于你自己的设备本地，不经过任何第三方服务器

---

## 🤝 贡献

欢迎提交 Issue 与 Pull Request。

- **Bug 报告**：请描述复现步骤与浏览器环境
- **功能建议**：在 Issue 中说明使用场景
- **代码贡献**：本项目保持单文件架构，请勿引入构建工具或外部依赖

---

## 📄 开源协议

[MIT License](./LICENSE) · 自由使用、修改与分发，保留原始署名即可。

---

## English

**Provenance** is a single-file HTML tool that helps you trace the real origin of a quote you vaguely remember, or transform your idea into a well-crafted expression backed by real citations.

**Core features:**
- **Trace**: Input your rough memory of a quote → get the verified original text, source, author, year, and confidence rating (with misattribution warnings)
- **Polish**: Input what you want to express → get (A) real citations from notable works you can actually attribute, and (B) original rewritten expressions in your own voice — strictly separated, never fabricated
- **Library**: Save, search, and export your collected quotes locally

**Setup**: Download `index.html`, open in any modern browser, enter your [DeepSeek API Key](https://platform.deepseek.com) in Settings. No install, no backend, no account required.

**Tech**: Vanilla HTML/JS · DeepSeek API · localStorage · Zero dependencies

---

<div align="center">

Built with vanilla HTML/JS · Powered by [DeepSeek](https://www.deepseek.com)

</div>
