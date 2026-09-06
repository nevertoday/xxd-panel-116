# Panel 116 runtime adapter

The canonical source brief is `references/original-prompt/zh-CN.md`. This adapter only records delivery variables; it never replaces the original aesthetic instructions.

- Modes: `top-bottom`, `left-right`, `design-only`, `wallpaper-pack`
- Ordinary comparison modes: strict 50:50 split; top-bottom keeps reality above, left-right keeps reality left.
- Text: `prompt`, `exact`, or `none`; resolve locale explicitly.
- Sizes: `auto`, `source`, common ratios, custom ratios, or exact pixels.
- Inputs: one image or an isolated directory batch.
