# cyrene ✦

> “如果故事走到了难过的一页，就先把它好好记住吧。春天还会回来，我们也一定会再见的♪”

`cyrene` 是一只住在 Codex 角落里的昔涟 Q 版动态宠物。

她不是严肃的代码审查官，也不会因为一次失败就皱着眉头追问原因。她更像是旅途中一直坐在你身边的故事讲述者：温柔、明亮，喜欢漂亮的事物和小小的仪式感；偶尔俏皮地眨眨眼，却比任何人都认真地珍惜相遇、约定与共同走过的时间。

对她而言，“浪漫”不只是甜蜜。明知道前路艰难，仍愿意和重要的人一起走下去；哪怕故事暂时没有完美结局，也要记得那些真实存在过的笑容——这才是她最相信的浪漫。

![cyrene 的完整动作预览](./contact-sheet.png)

## 她会怎样陪着你？

任务顺利时，她会挥手、跳起来，开心得像亲眼看见故事翻到了闪闪发亮的新一页。

任务失败时，她不会责怪你。她会短暂失落一下，然后继续留在原地：失败也是旅途的一部分，而你不需要独自面对它。

当 Codex 需要授权、输入或下一步决定时，她会安静地摊开手等待。不是催促，只是在说：“下一页要怎么写，由你决定。我会在这里。”

## 小小身体，动作很多

| 状态 | cyrene 的表现 |
| --- | --- |
| `idle` | 轻轻呼吸、眨眼，把此刻也收进记忆里 |
| `running-right` / `running-left` | 像追逐流星一样跟着任务赶路 |
| `waving` | 一看见你，就认真地打招呼 |
| `jumping` | 为每一个值得开心的小进展庆祝 |
| `failed` | 会难过，但不会把失败怪在你身上 |
| `waiting` | 耐心等待你决定故事的下一页 |
| `running` | 专注记录旅程，不让重要的瞬间溜走 |
| `review` | 把完成的成果捧到你面前，期待一起回顾 |

她还有一整圈 16 向注视。光标走到哪里，她的目光就会努力追到哪里——毕竟，真正想记住一个人时，总会忍不住多看几眼。

![cyrene 的 16 向注视](./look-directions.png)

## 安装

将 `pet.json` 与 `spritesheet.webp` 放入 Codex 的宠物目录：

```text
~/.codex/pets/cyrene/
├── pet.json
└── spritesheet.webp
```

Windows PowerShell：

```powershell
$petDir = Join-Path $env:USERPROFILE ".codex\pets\cyrene"
New-Item -ItemType Directory -Path $petDir -Force | Out-Null
Copy-Item .\pet.json, .\spritesheet.webp -Destination $petDir -Force
```

## 技术规格

- Codex pet schema：v2
- 图集尺寸：1536 × 2288
- 网格：8 列 × 11 行
- 单元格：192 × 208
- 图像格式：RGBA WebP
- 标准动画：9 行
- 注视方向：16 个
- 透明 RGB 残留：0
- 最终视觉验收：通过

完整机器校验见 [`validation.json`](./validation.json)，生成与验收摘要见 [`run-summary.json`](./run-summary.json)。

## 人设与视觉依据

官方角色预告中的 cyrene 珍视记忆与相遇。即使命运反复带来离别，她仍愿意守住希望、记得共同见过的风景，并相信春天终会回来。本宠物的性格据此调整为温柔、亲近、略带俏皮，同时在真正重要的事情上格外坚定。

- [官方角色预告：Cyrene — “With You Once More”](https://www.youtube.com/watch?v=CRAuK8T6Xis)
- [Sketchfab：Cyrene by Fella_001](https://sketchfab.com/3d-models/cyrene-615e7f6541ce492fa3db1f05e5438788) 提供可下载的 CC BY 角色模型，作为开放轮廓参考。
- 公开 Q 版图片仅用于视觉研究和风格理解，没有作为原始素材重新分发。
- 本仓库中的宠物图集由生成式图像流程重新创作，并经过结构、透明度、动作和方向视觉检查。

详细来源记录见 [`sources.md`](./sources.md)。

---

她不会承诺每一次运行都会成功。

但她会记得你们一起解决过的每一个问题，也会认真期待下一次重逢。♪
