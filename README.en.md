<div align="center">

# XXD Panel 116｜Pale-Paper Pastel Doodle Chronicle

Leave the photograph with a clear contour, easy colour, and a paper field that can breathe.

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## Sample works

The samples below use different original references. Panel 116 generated each one independently in a single pass, and AI metadata has been removed. Landscape samples are strict 50:50 left–right pairs with reality on the left and design on the right; portrait samples are strict 50:50 top–bottom pairs with reality above and design below.

**16:9 landscape · left–right 50:50**

| sample-05 | sample-06 |
|---|---|
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |

**3:4 portrait · top–bottom 50:50**

| sample-09 | sample-10 |
|---|---|
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## Best-fit situations and problems solved

What makes a photograph memorable is often not its information density, but one subject, one pose, a few colours, and a lingering emotion. **Panel 116** keeps the real photograph in the upper half and translates the lower half into pastel-crayon doodles on a very pale paper field: coarse contours, a few soft colour areas, minimal symbols, and a small-scale subject leave the composition room to breathe.

### Best for

- Keeping photographic identity and natural texture while gaining the ease and restraint of an art publication.
- Retaining only the core theme, relationships, and visual memories instead of tracing every object or filling the background.
- Bright, comforting pastel colour without muddiness, weak contrast, neon glare, or cheap candy sweetness.
- Consistent top-bottom, left-right, design-only, multi-ratio, wallpaper, or directory-batch delivery.

### What it solves

- Removes secondary information so detail and decoration do not swallow the subject.
- Keeps coloured lines clearly separate from the pale ground instead of letting the image dissolve into low contrast.
- Holds paired layouts to exactly two 50:50 regions with no title band, footer, or third section.
- Generates directly from each current original source, never from a sample, an intermediate result, or another Panel's output.

## Original prompt · five languages

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

The Chinese file preserves the user's original prompt verbatim and is the sole runtime creative and aesthetic authority. The other four files are complete, faithful reading translations and never rewrite the generation instructions.

**Signature:** very pale paper ground · coarse pastel-crayon contours · minimal doodle symbols · small-scale subject · 2–4 source-derived colours · clear coloured lines · generous artistic whitespace · vintage mechanical type

## Quick fit check

| What you need to know | What Panel 116 gives you |
|---|---|
| A clear relationship between photograph and design? | The real photograph remains above while a doodled translation of the same subject answers it below. |
| Recognition after abstraction? | It preserves the core theme, subject relationships, contour flow, pose, and colour memory first. |
| Pastels that do not turn grey? | A very pale ground, clear coloured lines, and a few soft blocks maintain readable contrast. |
| Flexible delivery sizes? | Common ratios, exact pixels, four modes, and directory batches are supported. |

## Transformation logic

```text
understand theme and relationships → distil contour, pose, direction, and emotion → remove secondary detail → rebuild with coarse crayon lines and sparse pastel blocks → place on pale paper with minimal doodle symbols → finish with whitespace and restrained mechanical type
```

## Recognisable finished traits

- A very pale, bright, clean near-white paper ground stays visibly lighter than all lines and colour areas.
- Subject contours are coarse, relaxed, dry, powdery, intermittently faded, slightly shaky, and incompletely closed.
- Surrounding symbols use one or only a few strokes; they never become polished icons, stickers, or standalone mini-illustrations.
- The subject remains small, off-centre, edge-adjacent, suspended, or locally cropped while whitespace actively composes the page.
- Two to four vivid, friendly colours distilled from the source become a bright, soft pastel-crayon palette.
- Sparse text uses airy, slightly irregular vintage mechanical typography rather than a fixed title template.

## Four output modes

- `top-bottom`: exactly two full-width regions, reality above and design below, 50% each.
- `left-right`: exactly two full-height regions, reality left and design right, 50% each; it never rotates into a top-bottom layout.
- `design-only`: the full canvas contains only Panel 116's designed translation; the photograph remains a non-visible reference.
- `wallpaper-pack`: creates complete artworks for phone, iPad, desktop, and watch, either `linked` as a coherent family or `independent` as four separate works.

Modes and sizes may be combined. Supported sizes include `1:1`, `3:4`, `4:3`, `4:5`, `5:4`, `2:3`, `3:2`, `9:16`, `16:9`, `21:9`, `5:7`, `7:5`, and exact pixels. Text can be prompt-generated, user-exact, or absent. A directory is inventoried recursively and every source is isolated while sharing one set of delivery settings; final PNG files remain flat in one fresh task directory.

## Getting started

```bash
git clone https://github.com/nevertoday/xxd-panel-116.git
npx skills add https://github.com/nevertoday/xxd-panel-116 --skill xxd-panel-116
```

Restart the agent session after installation, then invoke `$xxd-panel-116`. Add `--global --agent codex --yes` when a user-level Codex installation is wanted.

Common examples:

```text
/xxd-panel-116 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale en-US
/xxd-panel-116 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-116 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-116 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

See [SKILL.md](SKILL.md) for the full runtime contract and the [English](references/xxd-panel-116-prompt.en.md) or [Chinese](references/xxd-panel-116-prompt.zh-CN.md) runtime adapter.

<!-- xxd-readme-ads:start -->
## About XXD

XXD is Xiaoxiaodong's abbreviated brand name. Created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Support and membership

> **Advertising disclosure:** QR codes and paid membership/service links in this section are XXD promotional content. Scanning or purchasing is optional and does not affect access to this open-source project.

### Xiaoxiaodong Commander · General Command Skill · CNY 100

A one-time CNY 100 purchase unlocks this suite's General Command Skill (`xxd-panel-all`) for roster control, recommendations, Soldier dispatch, and batch coordination. Include “General Command Skill” in your WeChat message.

<!-- xxd-panel-command-system:start -->
**Your purchase unlocks the General Skill that commands the whole roster**

| Level | Skill | Responsibility |
|---|---|---|
| **General** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | Detect available numbered Skills; recommend by image, theme, or use; dispatch a chosen number; organize multi-style trials; and assign folders of images to individual jobs. |
| **Soldiers** | `xxd-panel-NNN` | Each numbered Skill executes only its own original brief and aesthetic, completing the individual job assigned by the General. |

The General Skill is the command center for the entire numbered-Skill roster. Your purchase unlocks it together with help for installation, updates, roster setup, and dispatch workflows. The General organizes and routes; it never rewrites, blends, or overrides a Soldier's original aesthetic. Every finished asset is still created independently by the selected Soldier Skill.
<!-- xxd-panel-command-system:end -->

### Knowledge Planet + Member Prompt Library + All General Skills Membership · CNY 699/year

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882), the [XXD Member Prompt Library](https://vip.xiaoxiaodong.ai/), and membership for all General Skills are one membership: **one annual payment unlocks all three benefits, with no second purchase required.**

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) · [Member Prompt Library](https://vip.xiaoxiaodong.ai/)

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD WeChat" width="280"></a></p>

---

<div align="center">

## Support this open-source project

If this project helps you, you’re welcome to support it through Buy Me a Coffee—entirely optional.

<p align="center"><a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Buy Me a Coffee" width="180"></a></p>

</div>
<!-- xxd-readme-ads:end -->

## License

This project—including the Skill, prompts, scripts, documentation, and accompanying sample images—is licensed under the **PolyForm Noncommercial License 1.0.0**. See [LICENSE](LICENSE) for the full legal text and <https://polyformproject.org/licenses/noncommercial/1.0.0> for the official page.

In plain language:

- Individuals may use it for study, research, experimentation, testing, hobby projects, and private entertainment. Charities, educational institutions, public research, safety or health organisations, environmental organisations, and government institutions may also use it.
- For **noncommercial purposes**, you may use, copy, modify, create derivative works, and share it. When sharing, you must also provide this license (or the link above) and every `Required Notice:` statement supplied by the author.
- It may not be used in commercial products or services, paid delivery, sale of access or licences, or any use expected to lead to commercial application. Obtain separate written permission from the copyright holder before commercial use.
- The agreement grants only the copyright licence and limited patent licence expressly stated. It grants no trademarks, brand names, or other unstated rights, and you may not sublicense your licence to others.
- After written notice of a violation, you must return to compliance and take practical remedial steps within 32 days, or the licences terminate immediately. A written patent-infringement claim also terminates the patent licence.
- The material is provided “as is”, without warranty to the extent permitted by law. Users bear the risks and potential losses arising from its use.
