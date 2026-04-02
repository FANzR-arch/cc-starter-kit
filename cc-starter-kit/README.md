# Claude Code Starter Kit

装好 Claude Code 之后的下一步——一套可以直接用的初始化系统。

包含：
- 初始化引导（让 CC 认识你，自动建立记忆文件）
- CLAUDE.md 模板（项目配置结构）
- Skill 示例（可复用的工作流模块）
- memory/ 目录模板

## 第一步：初始化

打开 Claude Code，把 `init.md` 里的全部内容复制进去，回车。

CC 会逐个问你 5 个问题，然后自动生成你的记忆文件和基础配置。整个过程大概 10 分钟。

## 第二步：看看生成了什么

初始化完成后，你的项目目录里会有：

```
memory/
  MEMORY.md           ← 记忆索引
  user_profile.md     ← 你的基本信息
  workflow_main.md    ← 你的主要工作流
  rules.md            ← 输出偏好和禁区
CLAUDE.md             ← 项目配置
```

打开这些文件检查一下，有不准确的地方直接手动改。

## 第三步：加入你自己的 Skill

`skills/examples/` 里有几个通用场景的 Skill 示例，参考结构写你自己的。

每个 Skill 是一个文件夹：

```
skill-name/
  SKILL.md        ← 触发条件 + 执行步骤
  references/     ← 这个任务要参考的素材（可选）
```

## 关于 CLAUDE.md

`CLAUDE.md` 放在项目根目录，Claude Code 启动时自动读取。

模板里的内容只是示例，按你自己的情况改。核心是写清楚：

- 你在这个项目里做什么
- 你有哪些常用工作流，用什么关键词触发
- 你的输出规范

---

有问题或建议，欢迎提 issue 或在 X 上找我 [@Formulasearch](https://x.com/Formulasearch)。
