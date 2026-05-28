# GitHub Profile 设计文档

**日期**: 2026-05-28
**用户**: heimaolala
**仓库**: heimaolala/heimaolala

## 概述

为 GitHub 个人主页创建视觉丰富的 README profile，采用视觉丰富型方案，包含动态打字机标题、贪吃蛇动画、统计卡片等元素。

## 风格定位

**混合型**：专业技术 + 个人特色。中英双语展示，中文优先。

## 配色方案

| 角色 | Hex | 用途 |
|------|-----|------|
| 奶白 | `#FEFAF6` | 卡片背底、大面积底色 |
| 橙色 | `#E8783B` | 图标、标题、高亮强调 |
| 灰 | `#ABAAA8` | 分隔线、装饰、次要文字 |
| 深灰 | `#333333` | 正文文字 |

## 布局结构（从上到下）

### 1. 头部横幅
- **打字机 SVG**: [readme-typing-svg](https://readme-typing-svg.herokuapp.com) 轮播 4 句文案：
  1. `Hi, I'm Heimaolala 👋`
  2. `你好，我是黑猫拉拉 🐱`
  3. `DL & LLM Enthusiast 🤖`
  4. `深度学习 & 大模型爱好者 📚`
- **波浪分隔线**: SVG 波浪过渡到下方内容
- 颜色: 橙色 `#E8783B`

### 2. 个人介绍
中英双语，层级展示：
- 🎓 北京邮电大学 · 数据科学与大数据技术 / *BUPT · Data Science & Big Data Technology*
- 🧠 专注于深度学习 & 大语言模型 / *Focused on Deep Learning & LLMs*
- ✨ "让模型理解世界" / *"Let models understand the world"*
- 📧 heimaolala@outlook.com · 🌐 [www.heimaolala.top](https://www.heimaolala.top)

### 3. 技术栈
使用 shields.io 徽章，分类分块展示：

| 类别 | 内容 |
|------|------|
| 🐍 Language | Python |
| 🔥 Framework | PyTorch |
| 🤖 AI & LLM | Transformers, DeepSpeed, HuggingFace, LoRA |
| 🛠 Tools | Git, Docker, Linux, Jupyter, VS Code |

### 4. 统计卡片 & 动态元素
- **三栏并排**: GitHub Stats / Streak / Top Languages（[github-readme-stats](https://github.com/anuraghazra/github-readme-stats)）
- **GitHub Trophy**: 成就奖杯
- 卡片配色: `bg_color=FEFAF6`, `title_color=E8783B`, `icon_color=E8783B`, `text_color=333333`

### 5. 贪吃蛇动画
- 使用 [snk](https://github.com/Platane/snk) 生成 SVG 动画
- 蛇身 #E8783B（橙色），食物 #ABAAA8（灰色）
- 通过 GitHub Actions 自动每日更新

### 6. 项目展示
- 占位，后续补充具体项目

### 7. 页脚
- 趣味语录: *"Fine-tuning myself, one commit at a time."*
- 可加 visitor count

## 外部依赖

| 服务 | 用途 |
|------|------|
| `readme-typing-svg.herokuapp.com` | 打字机标题 SVG |
| `anuraghazra/github-readme-stats` | 统计卡片 |
| `ryo-ma/github-profile-trophy` | 成就奖杯 |
| `Platane/snk` | 贪吃蛇动画 SVG |
| `shields.io` | 技术栈徽章 |

## 技术实现

- 仓库名: `heimaolala/heimaolala`（GitHub 特殊仓库，README 自动渲染到个人主页）
- 纯 Markdown + SVG 外链，无需构建
- 贪吃蛇使用 GitHub Actions 每日自动更新 SVG 输出
- 文件名: `README.md`

## 注意事项

- 动态 SVG 卡片依赖外部服务，加载速度可能有波动
- 贪吃蛇需设置 GitHub Actions workflow 并启用 GitHub Pages 或直接输出到仓库
- 所有外部图片链接务必使用 HTTPS
