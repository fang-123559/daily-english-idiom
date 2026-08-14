# memory.md 模板 — 配置与历史推荐记录

> 用途：Skill 的模板选择和去重机制都依赖此文件。
> 复制本文件到项目根目录并命名为 `memory.md`，每次推送后按「第四步：更新历史记录」维护。
> 注意：文件编码必须为 UTF-8。

# 每日英语俗语 - 执行记录

## 配置

- 卡片模板: A    <!-- 可选 A / B / C / F / G / I / J / K / ROTATE，预览与风格说明见 templates/cards/README.md；改这里即可换肤 -->

## 历史推荐（避免重复）

**重要：每次执行前必须检查此列表，严禁推荐已存在的俗语！**

| 日期 | 俗语 | 中文含义 |
|------|------|----------|
| 2026-06-24 | Face the music | 面对现实；承担后果；接受批评 |
| 2026-06-23 | Don't count your chickens before they hatch | 别高兴太早；不要过早乐观 |
| 2026-06-21 | The whole nine yards | 全部，所有，彻头彻尾，毫无保留 |
| 2026-06-20 | The squeaky wheel gets the grease | 会哭的孩子有奶吃；主动争取才能获得帮助 |
| 2026-06-18 | Pull someone's leg | 开玩笑；愚弄；戏弄 |

**已推送俗语列表（快速查看）**：
- Face the music
- Don't count your chickens before they hatch
- The whole nine yards
- The squeaky wheel gets the grease
- Pull someone's leg

---

## 执行日志

- YYYY-MM-DD：执行成功。推荐俗语 {俗语}，SVG 卡片按规范生成，结构化文字输出完整。历史记录已更新。

---

## 使用说明

1. **每次执行前**：
   - 读取「配置」区的 `卡片模板` 字段，确定本次使用的卡片模板
   - 读取「历史推荐」表格，获取所有已推送俗语，严禁推荐重复项
2. **每次执行后**：
   - 将新俗语、日期、中文含义追加到「历史推荐」表格
   - 同步更新「已推送俗语列表（快速查看）」
   - 在「执行日志」中追加一条记录
   - 确保文件编码为 UTF-8
3. **表格损坏时**：备份原文件，重建表格
