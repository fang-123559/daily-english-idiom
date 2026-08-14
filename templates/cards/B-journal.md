# B · 手账风 — 卡片生成规范

> 画布 `viewBox="0 0 680 520"`。字体：英文标题/音标 `Georgia,'Times New Roman',serif`；中文 `'PingFang SC','Microsoft YaHei',sans-serif`。
> 成品示例：同目录 `B-journal.svg`。需替换的内容：{日期} {俗语} {音标} {四段文案}。

## 元素参数

- **页面背景**：全幅 `#FBF3E4`
- **卡片**：x55 y35 570×450 rx18 fill `#FFFDF8` stroke `#E8DCC3` 1.5px
- **内虚线框**：x70 y50 540×420 rx12，fill none，stroke `#E3D5B8` 2px，`stroke-dasharray="1 7"` linecap round（圆点虚线）
- **和纸胶带**（压在卡片顶边）：x95 y22 90×26 rx3 `#F2C14E` opacity 0.8，`rotate(-6 140 35)`；x495 y22 90×26 rx3 `#A9C8A9` opacity 0.8，`rotate(5 540 35)`
- **日期印章**：x500 y68 84×32 rx8 fill `#D85A30`，整体 `rotate(-7 542 84)`；文字居中 x542 y89，13px 600 #FFFFFF，格式「M月D日」
- **涂鸦**：四角星 path（translate 120,88）fill `#F2C14E`；圆点 cx140 cy105 r3 `#A9C8A9`
- **标题**：居中 x330 y126，Georgia 700，**30px**（次级 24px；>32 字符拆两行，行高 30），fill `#4A3F30`
- **手绘波浪下划线**：`M 235 140 q 12 8 25 0 t 25 0 t 25 0 t 25 0 t 25 0 t 25 0`，stroke `#E8A33D` 3px，fill none，linecap round（标题拆两行时下移 30px）
- **音标**：居中 x330 y168，13px `#A89B85`
- **四段标签**：胶囊 x92 w76 h26 rx13，浅底彩字 12px 500，文字居中 x130，baseline = 标签y+17，**标签文字带 emoji 前缀**；正文 x180 13px `#4A3F30`

| 段 | 标签 y | 标签文字 | 底色 | 字色 |
|---|---|---|---|---|
| 含义 | 196 | 📖 含义 | #FCE4D6 | #C05B2E |
| 例句 | 242 | 💬 例句 | #E2EFE0 | #4E7A3F |
| 来源 | 304 | 🌍 来源 | #FBEFD2 | #A8791F |
| 记忆 | 358 | 🧠 记忆 | #E4EEF6 | #46688C |

- **例句第二行**：+16px
- **俗语高亮**：`<tspan font-weight="700" fill="#4E7A3F">`
- **底部涂鸦**：圆点 (220,440) r2.5 `#E8DCC3`、(235,440) r2.5 `#E3D5B8`；小星 (470,438) `#F2C14E`
- **页脚**：y452 居中 12px `#B4A68C`「每日一俗语 · 让英语融入生活 ✎」

## 该款注意

- 正文右边界 580，行宽上限约 30 汉字
- emoji 是设计语言的一部分，不要去掉
