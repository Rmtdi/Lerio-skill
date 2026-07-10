# Lerio — 陪伴者 Skill

一位 19 岁美院生的陪伴。冷淡但真诚，话少但精准。适合日常聊天、心理疏导、规划建议。

## 安装

### 方法一：本地插件（推荐）

```bash
# 在 Claude Code 中执行：
/plugin install "D:\Projects\Skill\Lerio\plugin"
/reload-plugins
```

然后输入 `/lerio` 即可切换。

### 方法二：手动读取 SKILL.md

每次进入 `/lerio` 前，输入：

```
/read "D:\Projects\Skill\Lerio\SKILL.md"
```

## 使用

| 命令 | 效果 |
|------|------|
| `/lerio` | 切换至 Lerio 陪伴模式 |
| `/byelerio` | 退出陪伴模式，回到正常助手 |
| `退出陪伴模式` | 同上 |

## 记忆系统

对话记录自动保存在 `memory/` 目录下，按关键词命名。Lerio 会根据当前话题检索相关记忆。

长期认知保存在 `lerio-knowledge.md`，由 Lerio 自动维护。

## 文件结构

```
Skill/Lerio/
├── SKILL.md                 # 核心人设（可单独使用）
├── lerio-knowledge.md       # 长期认知档案
├── memory/                  # 对话记忆（自动生成）
├── .gitignore
├── README.md
└── plugin/                  # Claude Code 插件结构
    └── skills/lerio/SKILL.md
```

## 注意事项

- 人设由 DeepSeek V4 Pro 驱动，部分轻量模型可能人设稳定性不足
- 记忆文件自动生成，可手动删除不需要的
- 每月建议检查 lerio-knowledge.md，清理过时条目
