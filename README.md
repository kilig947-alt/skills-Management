# skills-Management

可独立安装的 Agent Skills 集合。

## Skills

| Skill | 用途 |
| --- | --- |
| [product-art-direction](skills/product-art-direction/SKILL.md) | 为真实产品界面提供艺术指导与前端改造，根据任务和内容优化构图、视觉层级、排版与空间节奏。 |

## 安装

需要 Node.js 和 Git。在目标项目目录执行：

```bash
npx skills add kilig947-alt/skills-Management --skill product-art-direction
```

仅安装到 Codex：

```bash
npx skills add kilig947-alt/skills-Management --skill product-art-direction --agent codex
```

添加 `--global` 可安装到用户级目录。查看仓库中可安装的 skills：

```bash
npx skills add kilig947-alt/skills-Management --list
```

## 使用

安装后，在支持 Agent Skills 的工具中调用 `product-art-direction`，并提供目标页面、代码位置或参考图。例如：

> 使用 $product-art-direction 优化当前产品页面的构图、视觉层级和空间节奏，保留真实业务流程，并检查实际渲染效果。

Skill 强调真实数据、任务优先的布局、稳定的操作路径、主题继承，以及桌面和窄屏的实际渲染验证。

## 目录

```text
skills/
└── product-art-direction/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

每个子 skill 存放在 `skills/<skill-name>/`，并通过包含 `name` 和 `description` 的 `SKILL.md` 定义。`agents/openai.yaml` 提供显示名称和默认提示词。

## 在 skills.sh 中查找

```bash
npx skills find product-art-direction
```

[skills.sh 官方说明](https://skills.sh/docs/faq)：收录由真实的 `npx skills add` 安装遥测触发，搜索结果取决于平台索引更新。
