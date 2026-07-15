# 小晚蜡笔配图 Skill

为中文文章、帖子、博客、Notion 文档和方法论内容生成“小晚”蜡笔涂鸦绘本风的正文配图。

默认角色：粉色倒扣小桶、黑色短刘海、奶油碎花裙、焦糖棕背带裙、胡萝卜/兔子鞋。整体采用深蓝灰蜡笔线稿、颗粒填色和白底留白；不生成真人感、日系精修或光滑数字插画。

## 安装

```bash
git clone https://github.com/tianshuhao123-ai/my-ip-xiaowan.git
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./my-ip-xiaowan/xiaowan-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后，在 Codex 中使用：

```text
Use $xiaowan-illustrations 为这篇中文文章设计并生成 4 张小晚蜡笔绘本正文配图。
```

## 用法

先做策略：

```text
Use $xiaowan-illustrations 先不要生图，分析下面文章并输出 5 张配图 shot list。
```

生成单图：

```text
Use $xiaowan-illustrations 为“持续做一件小事，最后会长成结果”生成一张正文配图。
```

编辑图片：

```text
Use $xiaowan-illustrations 编辑这张图：把小晚改成正在浇一颗小种子，其他保持不变。
```

## 结构

```text
xiaowan-illustrations/
├── SKILL.md
├── agents/openai.yaml
├── assets/xiaowan-reference.png
└── references/
    ├── brand-dna.md
    ├── xiaowan-ip.md
    ├── composition-patterns.md
    ├── prompt-template.md
    └── qa-checklist.md
```

`assets/xiaowan-reference.png` 是唯一角色基准，生成小晚时必须使用。历史样例仅为原项目来源记录，不应作为小晚参考。

## 衍生来源与授权

本项目基于 Ian Xiaohei Illustrations 衍生，保留原始 MIT License 与 NOTICE 中的来源归属。小晚角色、参考图和定制规则属于本 Fork 的新增内容。
