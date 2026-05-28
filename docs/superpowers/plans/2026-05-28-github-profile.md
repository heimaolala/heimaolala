# GitHub Profile 实现计划

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 为 heimaolala 创建视觉丰富的 GitHub 个人主页 README。

**Architecture:** 单文件 `README.md`，纯 Markdown + 外部 SVG/Dynamic Card 引用。贪吃蛇动画通过 GitHub Actions 自动每日更新生成 SVG。

**Tech Stack:** Markdown, GitHub Actions (YAML), 外部动态 SVG 服务

**重要约束:** 中英文双语，默认中文在前。

---

### Task 1: 创建 README.md — 头部横幅 + 个人介绍 + 技术栈

**Files:**
- Create: `d:/vibeCoding/HeimaolalaProfile/README.md`

- [ ] **Step 1: 写 README.md 顶部区域（打字机标题、波浪线、介绍、技术栈）**

```markdown
<div align="center">

<!-- 打字机标题 -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.herokuapp.com/?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=E8783B&center=true&vCenter=true&random=false&width=600&lines=Hi,+I%27m+Heimaolala+%F0%9F%91%8B;%E4%BD%A0%E5%A5%BD%EF%BC%8C%E6%88%91%E6%98%AF%E9%BB%91%E7%8C%AB%E6%8B%89%E6%8B%89+%F0%9F%90%B1;DL+%26+LLM+Enthusiast+%F0%9F%A4%96;%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0+%26+%E5%A4%A7%E6%A8%A1%E5%9E%8B%E7%88%B1%E5%A5%BD%E8%80%85+%F0%9F%93%9A" alt="Typing SVG" />
</a>

<!-- 波浪分隔线 -->
<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" alt="wave" />

</div>

---

### 👋 关于我 / About Me

> 🎓 **北京邮电大学** · 数据科学与大数据技术  
> *BUPT · Data Science & Big Data Technology*  
>  
> 🧠 专注于**深度学习 & 大语言模型**  
> *Focused on Deep Learning & LLMs*  
>  
> ✨ "让模型理解世界"  
> *"Let models understand the world"*

📧 **heimaolala@outlook.com** · 🌐 [**www.heimaolala.top**](https://www.heimaolala.top)

---

### 🛠️ 技术栈 / Tech Stack

<p align="center">

<!-- Language -->
<b>🐍 Language</b><br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<br/><br/>

<!-- Framework -->
<b>🔥 Framework</b><br/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch" />
<br/><br/>

<!-- AI & LLM -->
<b>🤖 AI & LLM</b><br/>
<img src="https://img.shields.io/badge/Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="Transformers" />
<img src="https://img.shields.io/badge/DeepSpeed-000000?style=for-the-badge&logo=microsoft&logoColor=white" alt="DeepSpeed" />
<img src="https://img.shields.io/badge/%F0%9F%A4%97_HuggingFace-FFD21E?style=for-the-badge" alt="HuggingFace" />
<img src="https://img.shields.io/badge/LoRA-4B32C3?style=for-the-badge&logoColor=white" alt="LoRA" />
<br/><br/>

<!-- Tools -->
<b>🛠️ Tools</b><br/>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
<img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
<img src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code" />

</p>
```

- [ ] **Step 2: 本地预览验证**

在浏览器中打开或使用 Markdown 预览查看排版效果，确认：
- 打字机 SVG 可正常加载
- 中英文顺序正确（中文在前）
- 技术栈分类分块清晰
- emoji 正常渲染

---

### Task 2: 添加统计卡片 + 奖杯 + 贪吃蛇 + 页脚

**Files:**
- Modify: `d:/vibeCoding/HeimaolalaProfile/README.md`

- [ ] **Step: 在 README.md 末尾追加统计卡片、贪吃蛇、占位项目、页脚**

内容接在 Task 1 的技术栈之后：

```markdown
---

### 📊 GitHub 统计 / GitHub Stats

<p align="center">
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img height="160" src="https://github-readme-stats.vercel.app/api?username=heimaolala&show_icons=true&bg_color=FEFAF6&title_color=E8783B&icon_color=E8783B&text_color=333333&border_color=ABAAA8&rank_icon=github" alt="GitHub Stats" />
  </a>
  <a href="https://github-readme-streak-stats.herokuapp.com">
    <img height="160" src="https://github-readme-streak-stats.herokuapp.com/?user=heimaolala&background=FEFAF6&stroke=ABAAA8&ring=E8783B&fire=E8783B&currStreakNum=333333&sideNums=333333&currStreakLabel=333333&sideLabels=333333&dates=ABAAA8" alt="GitHub Streak" />
  </a>
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=heimaolala&layout=compact&bg_color=FEFAF6&title_color=E8783B&text_color=333333&border_color=ABAAA8" alt="Top Languages" />
  </a>
</p>

---

### 🏆 GitHub 奖杯 / GitHub Trophy

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=heimaolala&column=7&no-frame=true&no-bg=true&theme=flat&title_color=E8783B" alt="GitHub Trophy" />
</p>

---

### 🐍 贪吃蛇 / Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/heimaolala/heimaolala/output/snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/heimaolala/heimaolala/output/snake.svg" />
    <img src="https://raw.githubusercontent.com/heimaolala/heimaolala/output/snake.svg" alt="Snake animation" />
  </picture>
</p>

---

### 🚧 项目展示 / Projects

> *精选项目即将上线，敬请期待~*  
> *Featured projects coming soon!*

---

<div align="center">

*"Fine-tuning myself, one commit at a time."* 🐱

<img src="https://komarev.com/ghpvc/?username=heimaolala&color=E8783B&style=flat-square&label=Profile+Views" alt="Profile Views" />

</div>

<!-- 分隔线 -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=E8783B&height=120&section=footer" alt="footer wave" />
```

- [ ] **Step: 本地预览验证统计卡片颜色、贪吃蛇占位、页脚排版**

---

### Task 3: 创建贪吃蛇 GitHub Actions 工作流

**Files:**
- Create: `d:/vibeCoding/HeimaolalaProfile/.github/workflows/snake.yml`

- [ ] **Step: 写 GitHub Actions workflow**

```yaml
name: Generate Snake Animation

on:
  schedule:
    # 每天 UTC 0:00 自动运行
    - cron: "0 0 * * *"
  # 允许手动触发
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    permissions:
      contents: write

    steps:
      - name: Checkout
        uses: actions/checkout@v4

      - name: Generate snake SVG
        uses: Platane/snk@v3
        with:
          github_user_name: heimaolala
          outputs: |
            dist/snake.svg
            dist/snake.svg?palette=github-dark&color_snake=E8783B&color_dots=#ABAAA8,#ABAAA8,#ABAAA8,#ABAAA8,#ABAAA8

      - name: Push snake SVGs to output branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

- [ ] **Step: 确认 workflow 文件路径正确**

路径必须为 `.github/workflows/snake.yml`，推送到 GitHub 后会自动识别并定时执行。

---

### Task 4: 最终检查

- [ ] **Step 1: 全文检查 README.md**

逐项确认：
- [ ] 中性顺序：所有区块中文在前，英文在后
- [ ] 配色统一：`#FEFAF6` / `#E8783B` / `#ABAAA8` / `#333333`
- [ ] 所有外部图片链接 HTTPS
- [ ] 用户名正确：`heimaolala`
- [ ] 邮箱正确：`heimaolala@outlook.com`
- [ ] 博客地址正确：`www.heimaolala.top`

- [ ] **Step 2: 初始化 git 仓库并提交**

```bash
cd d:/vibeCoding/HeimaolalaProfile
git init
git add README.md .github/workflows/snake.yml docs/
git commit -m "feat: create GitHub profile README with dynamic elements"
```
