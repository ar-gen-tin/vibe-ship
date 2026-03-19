<div align="center">

# vibe-ship — 纯粹 Vibe 少踩坑

**给不懂代码的人的 AI 开发引导流程 — 从想法到发布**

[![Claude Code](https://img.shields.io/badge/Claude_Code-技能-blueviolet?logo=anthropic&logoColor=white)](https://claude.ai/claude-code)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

[English](README.md)

</div>

---

## 这是什么？

vibe-ship 是一个 Claude Code 技能，用问答的方式一步步带你从想法走到发布，即使你一行代码都不会写。

这个技能从三个真实项目（[Rockpile](https://github.com/nicekate/Rockpile)、[Spottt](https://github.com/ar-gen-tin/spottt)、[odds](https://github.com/ar-gen-tin/odds)）、60+ 个 bug、两次技术栈推倒重来、一次删库重建中提炼出来。

规则只有一条：**按顺序走，别跳步。**

---

## 八步流程

```
想清楚 → 问技术栈 → 最小版本 → 走通发布 → 安全扫描 → 做设计 → 砍功能 → 记录一切
  [1]      [2]        [3]        [4]        [5]        [6]       [7]       [8]
```

| 步骤 | 做什么 |
|------|--------|
| 1. **想清楚再开口** | 给谁用？核心功能是什么？最像的产品是什么？ |
| 2. **问技术栈** | 用什么做？为什么？有更好的方案吗？ |
| 3. **最丑但能用的版本** | 只做核心功能，不做设计，不做多语言，不做额外功能 |
| 4. **走通发布流程** | 签名、打包、部署，越早走通越不慌 |
| 5. **安全扫描** | 推送前检查密钥、邮箱、本地路径，不可跳过 |
| 6. **现在可以做设计了** | 最多 3 个方向，选一个做下去 |
| 7. **砍功能** | "这个不做，产品还能用吗？"能的话先别做 |
| 8. **记录一切** | AI 没有记忆，你替它记 |

---

## 安装

```bash
# 克隆到 Claude Code 技能目录
git clone https://github.com/ar-gen-tin/vibe-ship.git ~/.claude/skills/vibe-ship
```

或者手动把 `SKILL.md` 复制到 `~/.claude/skills/vibe-ship/` 目录下。

## 使用

```bash
/vibe-ship              # 从头开始
/vibe-ship --status     # 查看进度
```

---

## 这个技能会做什么

- 每一步都会问你问题，等你回答了再往下走
- 开发过程中你想加的额外功能会被记到「以后再说清单」，到第七步再审查
- 第五步安全扫描不可跳过
- 所有技术术语会被翻译成你能听懂的话
- MVP 完成后建议运行 `/code-review` 做代码质量检查
- 发布前可选运行 `/team` 做多角度审查

## 这个技能不会做什么

- 不教你写代码
- 不替你做产品决策（但会问你问题帮你想清楚）
- 不生成模板项目

---

## License

MIT

---

Don't Panic. Accelerate.
