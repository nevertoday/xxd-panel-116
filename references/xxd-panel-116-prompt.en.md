# Panel 116 runtime adapter

The canonical source brief is `references/original-prompt/zh-CN.md`. This adapter records delivery variables only and never replaces the original aesthetic instructions.

- Modes: `top-bottom`, `left-right`, `design-only`, `wallpaper-pack`
- Comparison modes use a strict 50:50 split: reality above for top-bottom and reality left for left-right.
- Text: `prompt`, `exact`, or `none`; resolve the target locale explicitly.
- Sizes: `auto`, `source`, common ratios, custom ratios, or exact pixels.
- Inputs: one image or an isolated directory batch.
