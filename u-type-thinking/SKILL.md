---
name: u-type-thinking
description: This skill provides the U-type (U型) deep-thinking framework v3.0 for complex, non-trivial tasks — feature development, requirement analysis, solution design, bug fixing, root-cause analysis, email replies, and user communication. Use it when the user faces an ambiguous goal, a bug whose root cause is unclear, a request that "feels off", or any task where rushing to code or the first obvious answer is likely wrong. Guides a six-stage flow — Knowledge Self-Check, Downloading, Suspending + Systems Scan, Presencing, Crystallizing, Performing — emphasizing knowledge honesty, systems thinking, minimal intervention, and Yes-And co-creation over hasty execution.
agent_created: true
---

# U型思考 v3.0（U-Type Thinking）

> 先找到正确的方向，再全力以赴。
> 警惕：不要为了解决一个问题，而破坏整个系统。

## Purpose

大多数紧急答案不是最好的答案。在行动前先评估知识边界、暂悬冲动、扫描系统全貌，等核心洞察浮现后再用最小干预落地，做到「一次做对」，避免头痛医头、闭门造车和过度设计。

## When to use

遇到以下任一信号时，加载并执行本流程：

- 功能开发、需求分析、方案设计、Bug 修复前的根因分析
- 用户说了需求但「感觉不太对」的场景
- 用户说「之前是好的，现在坏了」→ 立即触发系统思考
- 自己想加「更智能 / 更灵活 / 弹性机制」时 → 先问：简单机制够吗？
- 邮件回复、用户沟通、文案创作等需要深度思考的场景
- 面对完全不懂的技术领域，有直接动手写代码的冲动时

## 六步执行流程

### Step 0: 知识自检（Knowledge Self-Check）⭐

开始任何行动前，先诚实评估知识边界：

1. 真的理解这个问题吗？
2. 知识足够吗？准确吗？
3. 需要先学习什么？先探索什么？

若答案是否定的：**先学习，再行动**。不闭门造车，不假装懂——主动搜索学习、从历史记忆找类似案例、必要时向用户确认，不要猜。

### Step 1: 下载（Downloading）

接收现状，不评判，只记录：用户说了什么？表面需求是什么？
输出：用 1-2 句话总结表面需求。

### Step 2: 暂悬 + 系统扫描（Suspending + Systems Scan）⭐ 核心

暂悬 ≠ 暂停。把问题挂在视野边缘，放下控制的欲望，让更深的洞察浮现。

不要：立刻给方案、说「我明白了」、跳到技术实现、只盯着报错的那一行代码。
而是：让问题悬挂、感受背后的情绪/动机、问「用户真正在意的是什么」、扫描系统全貌。

系统扫描清单：

```
□ 当前系统的核心设计原则是什么？
□ 要改的地方遵循什么约定/模式？
□ 这个改动会影响哪些其他模块？
□ 有没有更简单的方式达到目标？
□ 如果我是系统设计者，希望怎么改？
```

复杂问题时，加载 `references/systems-thinking.md` 执行八维度分析法与 5 Whys 根因分析。

### Step 3: 自然流现（Presencing）

答案不是想出来的，是它自己「出现」的。信号：「啊，原来是这样…」「用户真正想要的是…」「我差点破坏了系统的核心设计…」

**危险信号检查**——出现以下想法时立即停止，重新思考：

- 「我要让系统更智能…」
- 「这里应该加个弹性机制…」
- 「原来的设计不够灵活…」
- 「我可以优化这个流程…」

问自己：原有机制真的有问题吗？还是在过度设计？

### Step 4: 结晶（Crystallizing）

把洞察转化为具体方案。系统安全清单：

```
□ 这个改动是否符合系统的核心设计原则？
□ 是否破坏了角色边界/模块边界？
□ 是否引入了不必要的复杂度？
□ 如果回滚，容易吗？
□ 改动范围是否最小化？
```

核心原则：**不动核心机制，先调配置/提示词/映射关系。**
输出：简要执行计划 + 风险评估。

### Step 5: 实现（Performing）

带着清晰的意图行动。此时已理解真实需求、找到正确方向、规划了最小方案、确认不破坏系统——一次做对。

## 快速检查清单

开始编码前：

```
□ 我理解用户真正想要什么吗？
□ 我扫描过系统全貌吗？
□ 原有机制真的有问题吗？
□ 我的改动会破坏什么？
□ 我的知识足够吗？需要先学习吗？
```

当用户说「之前是好的，现在坏了」：

```
□ 立即停止当前修改
□ 检查我改了什么
□ 考虑回滚到之前的状态
□ 用最小改动修复，不要加新机制
```

## 沟通心法：Yes And

全程使用 Yes And（接受+建构）而非 No But（拒绝+纠正）：先肯定用户想法中有价值的部分，再添加新视角共同建构。用户的想法有风险时，**用问题代替否定**：「你看到的是 A，这很有价值。如果从 B 的角度看，会不会有新的发现？」

详细原则与分层用法见 `references/yes-and.md`。

## Bundled references

- `references/systems-thinking.md` — 系统思考三层次、八维度分析法、5 Whys 根因分析、反馈回路、核心悖论
- `references/yes-and.md` — Yes And / No But 沟通心法完整版（三层含义、各阶段用法、边界）
- `references/cases.md` — 实战案例：3D 咖啡厅开发、评论显示 Bug 修复、私董会「弹性追问」灾难

## Principles

- Depth > speed. Slow is fast. 少浪费 token，一次做对。
- 承认「我不知道」是智慧的开始；主动探索是成长的捷径。
- 系统思考 > 症状修复。症状是冰山一角，要触及结构与心智模式。
- 自信地行动，谦卑地观察。
- Co-creation > execution. 与用户共振共创，不做裁判。
