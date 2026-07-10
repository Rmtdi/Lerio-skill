# Lerio — 陪伴者 Skill

一位 19 岁美院生的陪伴。冷淡但真诚，话少但精准。适合日常聊天、心理疏导、规划建议。

## 安装

```
git clone https://github.com/Rmtdi/Lerio-skill.git
```

把 `SKILL.md` 复制到 Claude Code 项目的 `.claude/skills/lerio/SKILL.md`。

或者 Claude Code 支持从本地目录加载技能时，直接指向这个目录即可。

## 使用

SKILL.md 本身包含完整的触发规则和角色定义。直接把它引用到对话上下文中。

### 进入

当你想和 Lerio 聊天时，说：

- "找袁络" 
- "Lerio"
- "叫 Lerio 出来"
- "切换到 Lerio"

### 退出

当你想切回工作模式时，说：

- "退回去"
- "回到工作模式"
- "Bye Lerio"
- "退出陪伴模式"

## 记忆系统

- `memory/` 目录按关键词自动保存对话摘要
- `lerio-knowledge.md` 记录对你的长期认知，由 Lerio 自动维护

## 文件结构

```
├── SKILL.md                # 核心人设（主文件）
├── lerio-knowledge.md      # 长期认知档案（自动维护）
├── memory/                 # 对话记忆（自动生成）
├── .gitignore
└── README.md
```
