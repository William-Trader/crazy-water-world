# 🚽 疯狂水世界 · 开局一个移动公厕

> **Crazy Water World: Start With a Floating Toilet** — a single-file HTML game that is a 1:1 parody of the mobile-game ads that keep showing up in your short-video feed.

[![License](https://img.shields.io/badge/license-PolyForm%20Noncommercial%201.0.0-blue)](LICENSE) [![Single File](https://img.shields.io/badge/build-none%20needed-brightgreen)](index.html) [![Deps](https://img.shields.io/badge/dependencies-0-orange)](index.html)

### ▶ [在线试玩 · Play in browser](https://william-trader.github.io/crazy-water-world/)

**当前版本：v0.2** · [全部发行版 / All releases](https://github.com/William-Trader/crazy-water-world/releases)

### 版本

| 版本 | 单文件下载 | 内容 | 发行版 |
| --- | --- | --- | --- |
| **v0.2**（当前） | [`crazy-water-world-v0.2.html`](versions/crazy-water-world-v0.2.html) | 连击、四技能、30+ 成就与图鉴、势力委托、本地排行榜、多结局 | [Release v0.2](https://github.com/William-Trader/crazy-water-world/releases/tag/v0.2) |
| v0.1（原版保留） | [`crazy-water-world-v0.1.html`](versions/crazy-water-world-v0.1.html) | 初版：单文件、三模式、九槽位、BOSS 战 | [Release v0.1](https://github.com/William-Trader/crazy-water-world/releases/tag/v0.1) |

> `index.html` 始终是最新版（在线试玩即 v0.2）。历史版本完整留在 `versions/`，可直接下载单文件离线玩。

### v0.2 更新内容

- **连击系统**：3 连击起有加成，5 连 1.5×、8 连 2× 并触发「暴击!」；伸手够不着会断连击
- **四技能栏**：数字键 1–4 释放，独立冷却与 HUD 显示
- **30+ 成就 + 图鉴**：打捞、战斗、生存、委托多线触发；图鉴收录模块与猛兽
- **势力与委托**：四大势力贸易 + 定期随机委托，奖励晶核/零件
- **本地排行榜**：前 8 名成绩存 localStorage（`cws_board`）
- **多结局**：按分数与净水评级给出不同结局文本
- **体验**：暂停/静音按钮、错误提示框、HUD 重排；快捷键 空格暂停 · B 改装 · T 势力 · Q 委托 · 1234 技能 · M 静音

---

## 中文

### 这是啥

有一天我刷短视频，刷到第 8000 个《疯狂水世界》的广告。

每个广告看起来都不一样，每个广告的主角都是「海水过滤器」，每个广告最后都是「点左下角下载，三分钟一局」。

**但是没有一个广告给过一秒实机演示。**

行吧。既然你们不做，我做。于是就有了这个 —— 一个 152 KB 的单文件 HTML（v0.2 为 215 KB），双击就打，零依赖、零构建、零后端、零埋点（这次是真的没有）。

### 游戏是真的能玩的

- **开局一个移动公厕。** 不是比喻，是你排污槽里的 0 代模块，名字就叫「移动公厕」。全部故事从这里开始。
- **打捞漂流物**：木板 🪵 废铁 🔩 塑料 🧴 绳索 🪢 破布 🧣 鱼获 🐟 零件 🔌 晶核 💠。点了才捞得到，站在筏子另一头够不着会飘一个「太远了！」。
- **九大槽位**：淡水 / 能源 / 氧气 / 食物 / 航行 / 防御 / 排污 / 人口 / 等级。一寸寸把公厕改成 S 级避难所。
- **版本打脸系统**：装上「电鳗发电机」，你的「海水过滤器」当场过时，效能掉到 34%。广告里没人会告诉你这件事。
- **鉴定员上门**：按你的净水设备评 S / A / B / C / D。
  - S 级：*「海水…不，这是潮汐级净水设备。请您跟我来，总统厨房这边请。」*
  - D 级：*「连过滤器都没有？甲板上躺着吧，末日不讲情面。」*
- **肥强**，本作灵魂人物，台词如下：*「……OK。……OK。……OK。」*
- **邻居把空调外机装进你家**，你可以选择忍了，或者一拳打穿墙壁（掉 12 耐久，但拿回尊严）。
- **终局**：击沉「水之都盟主 · 陈浩」的旗舰，夺下潮汐净水塔。*「就凭你这块破公厕，也敢在我的海面上打水？」*

### 三个模式

| 模式 | 说明 |
| --- | --- |
| 普通 | 轻松上手 |
| **广告模式** | 弹幕轰炸 + 扫描线 + 禁止暂停（按暂停键会被告知「广告模式禁止暂停」）|
| 硬核 | 失败物资全部清零 |

广告模式的弹幕是照着你刷视频的记忆做的：

- 「一天能看到八万种疯狂水世界的AI广告」
- 「这游戏我至少看过20种广告」
- 「愣是一秒实机演示都没有」

### 怎么玩

| 操作 | 说明 |
| --- | --- |
| 点击漂浮物 | 打捞 |
| 点击猛兽 | 反击（装了炮台会自动开火）|
| 点击幸存者 | 收留（要有空床位和 12 食物）|
| 空格 | 暂停（广告模式下会被拒绝）|
| B | 改装面板 |

### 运行

```bash
git clone https://github.com/William-Trader/crazy-water-world.git
open crazy-water-world/index.html   # macOS
# 或者直接把 index.html 拖进浏览器
```

没有 npm install，没有 http server，没有环境变量。就一个文件。

### 技术

- 单文件 HTML：v0.2 约 3,665 行 / 215 KB（v0.1 为 2,992 行 / 152 KB），HTML + CSS + 原生 JS，无框架
- Canvas 2D 渲染，1280×720 逻辑分辨率，按 16:9 自适应缩放，横屏移动端可玩
- 程序化 BGM 与音效：WebAudio 现场合成，**仓库里没有一个音频文件**
- 最高分存 localStorage（key `cws_best2`）

---

## English

### What this is

One day I was scrolling short videos and hit the 8,000th ad for a game called *Crazy Water World*. Every ad looked different, every ad was centered on the same *seawater filter*, and every ad ended with *tap the bottom-left corner, three minutes per run*.

**Not one of those ads ever showed a single second of actual gameplay.**

Fine. You won't make it, so I did. The result is a 152 KB single-file HTML game (215 KB as of v0.2): no dependencies, no build step, no backend, and — for real this time — no telemetry.

### It actually plays

- **You start with a floating toilet.** Not a metaphor: it is the generation-0 module in your waste slot, literally named "Mobile Toilet". The whole story starts there.
- **Salvage the drift**: wood, scrap iron, plastic, rope, cloth, fish, parts, crystal cores. Click to collect — reach too far and it says *"too far!"*
- **Nine slots**: fresh water / energy / oxygen / food / navigation / defense / waste / population / grade. Turn the toilet into an S-tier shelter, one plate at a time.
- **Version-slap system**: install the *Electric Eel Generator* and your *Seawater Filter* instantly becomes obsolete — output drops to 34%. The ads never mention this.
- **The Inspector visits** and grades your water setup S / A / B / C / D. Grade S: *"Seawater… no, this is a tidal-class purification unit. Right this way, the President's Kitchen."* Grade D: *"No filter at all? Lie on the deck then. The apocalypse shows no mercy."*
- **Fei Qiang**, the soul of the game, delivers the line: *"…OK. …OK. …OK."*
- **Your neighbor installs an AC compressor in your floor.** You can let it slide, or punch through the wall (lose 12 durability, regain your dignity).
- **Finale**: sink the flagship of *Chen Hao, Warlord of the Water City*, and take the Tidal Purification Tower.

### Three modes

- **Normal** — easy going.
- **Ad Mode** — bullet-comment bombardment, scanlines, and pausing is *disabled* (the game will refuse).
- **Hardcore** — all resources wiped on failure.

### Controls

Click drifts to salvage · click beasts to fight back (cannons fire automatically) · click survivors to rescue · `Space` pause · `B` upgrade panel.

### Versions

| Version | Single file | Highlights | Release |
| --- | --- | --- | --- |
| **v0.2** (current) | [`crazy-water-world-v0.2.html`](versions/crazy-water-world-v0.2.html) | Combo meter, 4 active skills, 30+ achievements & codex, faction quests, local leaderboard, multiple endings | [v0.2](https://github.com/William-Trader/crazy-water-world/releases/tag/v0.2) |
| v0.1 (original, preserved) | [`crazy-water-world-v0.1.html`](versions/crazy-water-world-v0.1.html) | First release: three modes, nine slots, boss fight | [v0.1](https://github.com/William-Trader/crazy-water-world/releases/tag/v0.1) |

`index.html` always points at the latest build (GitHub Pages = v0.2); every past version stays in `versions/` as a downloadable single file.

### Run it

```bash
git clone https://github.com/William-Trader/crazy-water-world.git
open crazy-water-world/index.html
```

No npm install. No dev server. No env vars. It is one file.

### Tech

- Single-file HTML: ~3,665 lines / 215 KB in v0.2 (2,992 lines / 152 KB in v0.1), vanilla JS + Canvas 2D, no framework
- 1280×720 logical resolution, 16:9 letterboxed scaling, landscape mobile supported
- Procedural BGM and SFX synthesized live with WebAudio — **the repo contains zero audio files**
- Best score persisted in localStorage (`cws_best2`)

---

## License

**PolyForm Noncommercial License 1.0.0** — source-available. Read it, learn from it, fork it for fun and non-commercial use. **Commercial use is not permitted.** (This is *not* an OSI-approved open-source license; it is source-available by design.)

## Disclaimer

This is a parody / fan-made meme project. It is not affiliated with, endorsed by, or connected to any real game, studio, or advertiser. All characters and any resemblance to actual persons are fictional and played for laughs. 本项目纯属整活，与任何厂商、任何真人无关。
