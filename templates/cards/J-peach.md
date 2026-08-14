# J · 蜜桃盐系 — 卡片生成规范

> 画布 `viewBox="0 0 680 520"`。字体：英文标题/音标 `Georgia,'Times New Roman',serif`；中文 `'PingFang SC','Microsoft YaHei',sans-serif`。
> 成品示例：同目录 `J-peach.svg`。需替换的内容：{日期} {俗语} {音标} {四段文案}。

## 元素参数

- **页面背景**：全幅 `#FFF6F2`
- **底部双层波浪**（在卡片下层）：path1 `M 0,478 Q 85,458 170,478 T 340,478 T 510,478 T 680,478 L 680,520 L 0,520 Z` fill `#FFE4DC`；path2 同形 y+14，`#FFD0C4` opacity 0.55
- **卡片**：x75 y45 530×430 rx28 fill `#FFFFFF`；投影 `feDropShadow dy8 blur18 #F4AFA0 30%`
- **彩旗**：绳 `M 100,58 Q 310,96 520,58` stroke `#E8B4A6` 1.5px fill none；5 面三角旗（w24 h24，顶点向下，贴绳悬挂）y≈70/75/77/75/70，颜色依次 `#FFB4A2 / #FFD0C4 / #FF9E8A / #FFC9B8 / #F4A48E`
- **日期徽章**：外圈 cx572 cy72 r28 fill none stroke `#FF8FA3` 1.5px `stroke-dasharray="3 3"` opacity 0.45；内圆 r24 fill `#FF8FA3`；文字居中「M.D」格式（如 6.18）Georgia 700 13px #FFFFFF y77
- **标题**：居中 x340 y145，Georgia 700，**33px**（次级 26px；>32 字符拆两行，行高 33），fill `#3D2C29`
- **音标**：居中 x340 y172，14px `#B09A92`
- **强调条**：x310 y184 60×4 rx2，`#FFB4A2`
- **分隔**：x110→570，y196，圆点虚线 `#F6D9D0` 2px，`stroke-dasharray="2 6"` linecap round
- **四段标签**：统一胶囊 x100 w64 h26 rx13，fill `#FFEDE8`，文字 12px 600 `#E06B54` 居中 x132；正文 x180 13px `#5A4640`

| 段 | 标签 y | 文字 baseline |
|---|---|---|
| 含义 | 212 | 229 |
| 例句 | 258 | 275（第二行 291） |
| 来源 | 310 | 327 |
| 记忆 | 364 | 381 |

- **俗语高亮**：`<tspan font-weight="700" fill="#E06B54">`
- **页脚**：y450 居中 12px `#C4A99E`；两侧小圆点 (248,446) (432,446) r2.5 `#FFD0C4`

## 该款注意

- 单色系设计语言：四段标签同色同款是刻意的，不要给各段换不同颜色
- 日期徽章用「M.D」点分格式（6.18），不是「6月18日」
- 标题拆两行时：基线 y126 / y159，音标 y186，强调条 y198，分隔 y210，四段整体 +14 顺排；页脚不动
