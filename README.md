# 我的 Claude Skills 仓库

这里收录了我在使用 Claude 过程中沉淀下来的自定义 Skill，每个 Skill 封装了一类重复性任务的完整工作流，可直接安装到 Claude 中调用。

## 目录结构

```
/
├── README.md                        ← 你在这里
└── dolphindb-plugin-article/
    └── SKILL.md
```

---

## Skills 列表

### 📝 [dolphindb-plugin-article](./dolphindb-plugin-article/SKILL.md)

**用途**：根据 DolphinDB 插件/模块信息问卷，自动撰写一篇结构统一的微信公众号推文，用于 DolphinDB Marketplace 生态宣传。

**适用场景**：
- 开发者填写完插件介绍问卷后，需要快速生成宣传推文
- 需要保持多篇插件推文风格、结构、结尾完全一致

**输入**：填写好的 `.docx` 问卷文件（或等效的插件介绍材料）

**输出**：包含标题、痛点开篇、核心亮点、代码示例、适用场景、立即体验、共建生态等 8 个板块的 Markdown 推文文件

**触发关键词**：插件推文、模块推文、生态宣传、写一篇推文、DolphinDB 插件介绍

---

## 如何安装 Skill

1. 下载对应 Skill 文件夹
2. 在 Claude 中上传安装，或将文件夹路径挂载到 `/mnt/skills/user/` 目录下
3. 在对话中使用触发关键词即可自动调用

---

## 贡献新 Skill

如需添加新 Skill，请按以下结构新建文件夹：

```
your-skill-name/
└── SKILL.md          ← 必须，包含 YAML frontmatter 和 Skill 正文
```

并在本 README 的"Skills 列表"中补充对应条目。
