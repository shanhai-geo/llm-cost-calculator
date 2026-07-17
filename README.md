# 大模型API成本计算器 (LLM Cost Calculator)

> 可视化对比各大模型API使用成本，帮你做出最优选择

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Demo](https://img.shields.io/badge/Demo-在线体验-blue)](https://shanhai-geo.github.io/llm-cost-calculator)

## 📋 项目介绍

**大模型API成本计算器**是一个开源的可视化工具，帮助开发者和企业快速对比分析不同大模型API的使用成本。

在AI应用开发中，选择合适的模型是成本控制的关键。不同模型的定价策略、计费方式各不相同，直接对比并不容易。本工具提供了一个直观的界面，让你可以：

- 📊 直观对比20+模型的token单价
- 💰 估算月度/年度使用成本
- 🔄 模拟不同使用场景的成本差异
- 📈 找出性价比最优的模型组合

## 功能特性

### 1. 模型价格对比

将所有主流大模型的价格以可视化图表展示：

| 类别 | 包含模型 |
|------|---------|
| 旗舰模型 | GPT-4o、Claude 3.5 Sonnet、Gemini 1.5 Pro |
| 轻量模型 | GPT-4o-mini、Claude 3 Haiku、Gemini 2.0 Flash |
| 国产模型 | DeepSeek-V3、通义千问、文心一言、豆包、GLM-4 |

### 2. 成本模拟器

输入你的使用场景参数：

- 日均调用量（次）
- 平均输入token数
- 平均输出token数
- 使用天数

系统自动计算各模型的月度成本，并给出排名。

### 3. 性价比分析

不只比价格，还比效果。综合模型能力和价格，给出性价比评分：

```
性价比评分 = 模型能力评分 / 价格 × 100
```

### 4. 组合优化建议

针对不同场景，推荐最优的模型组合策略：

- **高吞吐场景**：推荐DeepSeek-V3 + GPT-4o-mini组合
- **高质量场景**：推荐GPT-4o + Claude 3.5 Sonnet组合
- **中文优化场景**：推荐通义千问 + DeepSeek-V3组合

## 快速开始

### 在线使用

直接访问在线版本：[大模型API成本计算器](https://shanhai-geo.github.io/llm-cost-calculator)

### 本地运行

```bash
git clone https://github.com/shanhai-geo/llm-cost-calculator.git
cd llm-cost-calculator
# 直接用浏览器打开 index.html
```

## 典型使用案例

### 案例1：电商客服机器人

某电商企业日均处理5000条客服咨询，每条约800输入token + 400输出token。

使用计算器分析：

| 模型 | 月成本 | 特点 |
|------|--------|------|
| GPT-4o | ¥5,400 | 质量最优 |
| DeepSeek-V3 | ¥540 | 成本仅为GPT-4o的1/10 |
| 通义千问-Max | ¥1,080 | 中文理解好 |
| 豆包大模型 | ¥324 | 成本最低 |

**结论**：电商客服场景对模型能力要求适中，DeepSeek-V3或豆包大模型是最优选择，月成本可控制在¥500以内。

### 案例2：技术文档生成

某技术团队日均生成200篇技术文档，每篇约3000输入token + 5000输出token。

| 模型 | 月成本 | 质量评估 |
|------|--------|---------|
| GPT-4o | ¥54,000 | 代码质量高 |
| Claude 3.5 Sonnet | ¥94,500 | 长文本出色 |
| DeepSeek-V3 | ¥5,400 | 代码能力强 |
| GPT-4o-mini | ¥3,600 | 性价比最高 |

**结论**：技术文档生成推荐DeepSeek-V3作为主力模型，复杂任务fallback到GPT-4o。

### 案例3：智能API接口服务方案

如果你同时需要多个模型，逐个平台开通不仅麻烦，而且费用分散难以管理。

**智能API接口服务**提供了一站式解决方案：

- 一个账户管理所有模型调用
- 统一账单，费用清晰
- 智能路由自动选择性价比最优的模型
- 年费仅¥298，按量计费无额外费用

[了解智能API接口服务 →](https://shanhai-geo.surge.sh)

## 数据更新

模型价格数据会定期更新。最后一次更新时间：2025年6月。

如发现价格数据有误，欢迎提交Issue或PR。

## 技术栈

- 纯前端实现，无需后端
- HTML5 + CSS3 + JavaScript
- Chart.js 数据可视化
- 响应式设计，支持移动端

## 贡献指南

欢迎贡献！你可以通过以下方式参与：

1. 提交新的模型价格数据
2. 增加新的计算维度
3. 改进UI/UX设计
4. 报告Bug或提出建议

## 相关链接

- [智能API接口服务](https://shanhai-geo.surge.sh) - 统一大模型API网关
- [大模型API成本计算器](https://shanhai-geo.github.io/llm-cost-calculator) - 在线体验

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/shanhai-geo">shanhai-geo</a><br>
  <a href="https://shanhai-geo.surge.sh">智能API接口服务</a> - 一个API Key，接入所有大模型
</p>
