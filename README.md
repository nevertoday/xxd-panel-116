<div align="center">

# XXD Panel 116｜浅纸粉彩涂鸦志

让照片留下清楚的轮廓、轻松的色彩和一块会呼吸的纸面

<strong>简体中文</strong> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## 样张展示

本项目已发布 8 张实际样片，图片文件位于 `assets/examples/`。

| sample-05 | sample-06 |
| --- | --- |
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| sample-07 | sample-08 |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |
| sample-09 | sample-10 |
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| sample-11 | sample-12 |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 适用场景与解决的问题

有些照片真正动人的不是信息量，而是一个主体、一段姿态、几种颜色和照片留下的情绪。**Panel 116** 保留上半部分的真实照片，再把下半部分转译成极浅纸面上的粉彩蜡笔涂鸦：粗颗粒轮廓、少量柔和色块、极简符号和小尺度主体共同留出呼吸感。

### 适合这些情况

- 想保留照片的身份与自然质感，同时得到更轻松、更像艺术出版物的海报。
- 不想逐物描摹、写实转绘或把背景塞满，只想留下核心主题、关系和视觉记忆点。
- 喜欢明亮治愈的粉彩色，但不接受灰暗、低对比、荧光或廉价糖果感。
- 需要同一套风格稳定输出上下、左右、纯设计、多比例、四端壁纸或目录批处理。

### 它替你解决什么

- 把复杂照片中的次要信息删掉，避免主体被细节和装饰吞没。
- 用清晰彩线与浅纸底保持识别度，避免背景和主体糊在一起。
- 让对照构图严格只有两个 50:50 区域，不出现标题带、底栏或第三分区。
- 每张图从当前原图一次直达生成，不把样张、中间结果或其他 Panel 作品再次送入模型。

## 使用窍门

- **先给一张清楚的照片：** 先选一张主体、动作和关系都容易辨认的图，再决定输出方式与比例。
- **一句话串起参数：** 直接说“上下对照 / 左右对照 / 纯设计 + 16:9 / 3:4 / 手机壁纸”，也可以补充电脑、平板或电子手表尺寸。
- **把必须保留的内容说清楚：** 指定人物、物件、动作、关系和文字；避免同时规定过多布局细节，让风格有空间完成设计。
- **文字有三种选择：** 让模型按图片智能生成、用 `--text exact --copy` 锁定逐字文案，或用 `--text none` 完全不要文字。
- **说明现实区与设计区：** 上下或左右对照时，注明哪一侧保留照片、哪一侧负责设计转译；纯设计和壁纸则说明整张画布都要重新设计。
- **先单张试，再批量做：** 先用一张图确认模式、比例、文字和语言，再把同一套参数用于目录批处理；每轮只改一个变量，结果更容易比较。

## 开始使用

```bash
git clone https://github.com/nevertoday/xxd-panel-116.git
npx skills add https://github.com/nevertoday/xxd-panel-116 --skill xxd-panel-116
```

安装后重新启动 Agent 会话，然后调用 `$xxd-panel-116`。也可以按需追加 `--global --agent codex --yes` 做用户级安装。

常用调用示例：

```text
/xxd-panel-116 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale zh-CN
/xxd-panel-116 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-116 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-116 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

完整运行契约见 [SKILL.md](SKILL.md)；运行适配器见 [英文](references/xxd-panel-116-prompt.en.md) 与 [中文](references/xxd-panel-116-prompt.zh-CN.md)。

## 原始提示词 · 五种语言

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中文文件逐字保存用户提供的原始提示词，是运行时唯一的创作与审美权威。其他四个版本是完整、忠实的阅读译文，不会反向改写生图指令。

**关键词：** 极浅纸面 · 粗颗粒粉彩蜡笔轮廓 · 极简涂鸦符号 · 小尺度主体 · 2–4 色照片取色 · 清晰彩线 · 大量艺术留白 · 旧式机械印字

## 快速判断：Panel 116 适合你吗？

| 你关心的问题 | 这套风格给你的回答 |
|---|---|
| 想要照片与设计之间有清楚的关系？ | 上方保留真实照片，下方以同一主体的涂鸦转译回应它。 |
| 担心抽象后认不出原物？ | 优先保留核心主题、主体关系、轮廓走势、姿态和色彩记忆。 |
| 喜欢粉彩但不想画面发灰？ | 采用极浅背景、清晰彩线和少量柔和色块，保持足够对比。 |
| 需要多种交付尺寸？ | 支持常用比例、准确像素、四种模式和目录批量。 |

## 四种输出模式

- `top-bottom`：整张画布只有上下两个全宽区域，现实照片在上、设计在下，严格各占 50%。
- `left-right`：整张画布只有左右两个全高区域，现实照片在左、设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现 Panel 116 的设计转译，照片只作为不可见参考。
- `wallpaper-pack`：按手机、iPad、桌面和手表分别生成完整设计壁纸，可选 `linked` 连贯套装或 `independent` 四张独立。

支持多选模式与比例（`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5` 或准确像素），以及模型生成文字、准确文字和无文字。传入目录会递归扫描图片，每张源图独立处理，共用一次交付设置；最终 PNG 平铺放入一个新任务目录。

<!-- xxd-readme-ads:start -->
## 关于 XXD

XXD 是小小东品牌名的缩写，本项目由小小东创建并维护：[@xiaoxiaodong01](https://x.com/xiaoxiaodong01)。

## 小小东多端会员 · 699 元/年

> **广告与商业信息声明：** 以下二维码、会员与付费服务链接属于小小东的广告信息。是否扫码或购买完全自愿，不影响本开源项目的访问与使用。

一次年费，同时开通三项会员权益：**知识星球 + 小小东成员提示词库 + 全部 将军总指挥 Skills 会员**。三项权益合并在同一份会员中，无需分别购买。

<!-- xxd-panel-command-system:start -->

### Skills 如何协作

| 层级 | 包含内容 | 用途 |
|---|---|---|
| **General** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 识别可用的编号 Skills，按图片、主题和用途推荐，并组织多风格试稿与批量任务。 |
| **Soldier** | `xxd-panel-NNN` | 每个编号执行自己的原始提示词与审美，完成 General 分派的具体任务。 |

<!-- xxd-panel-command-system:end -->

### 会员权益

1. **微信一对一 AI 学习与项目答疑**
   扫描下方二维码，添加小小东微信，围绕 AI 学习、工具使用和实际项目进行一对一沟通，获得答疑与建议；代表性问题将整理为会员内容。
2. **持续更新的成员提示词库**
   [小小东成员提示词库](https://vip.xiaoxiaodong.ai/)当前约有 3.2 万条提示词，会持续整理和扩充，目标超过 10 万条。
3. **全部 将军总指挥 Skills 与使用答疑**
   一份会员覆盖全部 将军总指挥 Skills；使用过程中遇到问题，可以获得相应的使用说明与答疑。
4. **高频刚需优先处理**
   会员提出的高频、刚需提示词与 Skills 需求，会优先评估和开发。

### 如何开通

- 可在[成员网站](https://vip.xiaoxiaodong.ai/)自助开通。
- 也可以扫描下方二维码，添加小小东微信，进行一对一沟通并获得开通协助。

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="联系小小东" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## 许可证

本项目（包括 Skill、提示词、脚本、文档及随附样张）采用 **PolyForm Noncommercial License 1.0.0**。完整法律条文请见 [LICENSE](LICENSE)，官方页面见 <https://polyformproject.org/licenses/noncommercial/1.0.0>。

用人话说：

- 个人可以用于学习、研究、实验、测试、兴趣项目和私人娱乐；慈善机构、教育机构、公共研究/安全/卫生机构、环保组织及政府机构也可以使用。
- 在**非商业目的**下，你可以使用、复制、修改、制作衍生作品并分享；分享时必须同时提供本许可证（或上面的链接）以及作者提供的所有 `Required Notice:` 声明。
- 不允许用于商业产品或服务、收费交付、出售访问权或许可，或任何预期会带来商业应用的用途。需要商业使用时，请先向版权方另行取得书面许可。
- 本协议只授予其中明确写出的著作权许可和有限的专利许可，不授予商标、品牌名称或其他未明确授予的权利，也不能把你的许可再转授给他人。
- 如果收到书面违约通知，须在 32 天内纠正并采取实际补救措施，否则许可会立即终止；就专利侵权提出书面主张也会终止专利许可。
- 内容按“现状”提供，在法律允许的范围内不作任何担保，使用风险和可能的损失由使用者自行承担。
