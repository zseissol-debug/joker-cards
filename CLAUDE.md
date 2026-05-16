# 小丑牌 Web · CLAUDE.md

## 项目定位

Vibe Coding 课程实战项目——用 AI 全流程开发一款 Balatro-like 单机网页游戏。目标是让零基础学员亲手体验「需求 → 设计 → 开发 → 测试」完整链路。

## 目录结构

```
.
├── game.html       # 游戏主文件（单文件，双击即玩）
├── PRD.html        # 产品需求文档 V1.0.0
├── DESIGN.html     # 视觉设计规范（Design Tokens + 组件）
├── agents/         # Claude Code 自定义 Agent（fullstack-engineer 等）
└── slash/          # Claude Code 自定义斜杠命令（cc-commit 等）
```

## 常用命令

```bash
# 打开游戏
open game.html

# 查看产品文档
open PRD.html

# 查看设计规范
open DESIGN.html
```

## 开发约定

- 游戏逻辑全部在 `game.html` 单文件内，不拆分文件
- 样式使用 CSS 变量（定义在 `:root`），颜色改动改变量即可
- 计分公式：`(基础分 + 选中牌点数之和) × 倍数`
- 牌型优先级从高到低：皇家同花顺 > 同花顺 > 四条 > 葫芦 > 同花 > 顺子 > 三条 > 两对 > 对子 > 高牌

## V1.0.0 明确不做

- 小丑牌 / 星球牌 / 增益系统
- 商店 / 关卡 / 盲注体系
- 动画 / 音效 / 粒子特效
- 多人联机

## 下一步路线

- v1.1.0：视觉升级（暗色风格 / Toast / 进度条）
- v1.2.0：小丑牌系统（8 张 Joker / 槽位 / 稀有度）
