<div align="center">

# XXD Panel 116｜淡紙パステル落書き誌

写真に、明快な輪郭と軽やかな色、呼吸できる紙面を残す。

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <strong>日本語</strong> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## サンプル展示

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

## 向いている場面と解決する課題

写真を記憶に残すのは情報量ではなく、一つの主体、姿勢、いくつかの色、そして残る感情であることがあります。**Panel 116** は上半分に実写を保ち、下半分を極めて淡い紙面のパステルクレヨン落書きへ翻訳します。粗い輪郭、少量の柔らかな色面、最小限の記号、小さな主体が余白に呼吸を与えます。

### こんな場合に

- 写真の個性と自然な質感を残しながら、アート出版物のように軽やかなポスターにしたい。
- 全ての物を描き写したり背景を埋めたりせず、主題、関係、記憶に残る形だけを残したい。
- 明るく癒やされるパステルが好きだが、灰色、低コントラスト、蛍光色、安いキャンディー感は避けたい。
- 上下、左右、デザインのみ、複数比率、4端末壁紙、フォルダ一括を同じ方向性で出力したい。

### 解決すること

- 二次情報を削り、細部や装飾に主体を埋もれさせません。
- 淡い紙面と明快な色線で識別性を保ち、背景と主体を同化させません。
- 比較レイアウトを二つの50:50領域だけに固定し、タイトル帯や第三の帯を作りません。
- 常に現在の原画像から一度で生成し、サンプルや中間結果、他 Panel の作品を再入力しません。

## 原文プロンプト · 5言語

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中国語ファイルはユーザーの原文を一字一句保存し、実行時の唯一の創作・美的権威です。他の4ファイルは完全で忠実な閲覧用翻訳であり、生成指示を書き換えません。

**特徴語：** 極淡の紙面 · 粗いパステルクレヨン輪郭 · 最小限の落書き記号 · 小さな主体 · 写真由来2–4色 · 明快な色線 · 大きな余白 · 古い機械印字

## クイック判定

| 気になること | Panel 116 の答え |
|---|---|
| 写真とデザインの関係を明確にしたい | 上に実写を残し、同じ主体の落書き翻訳を下で応答させます。 |
| 抽象化しても認識できるか | 主題、関係、輪郭の流れ、姿勢、色の記憶を優先して残します。 |
| パステルが灰色にならないか | 極淡の背景、明快な色線、少量の柔らかな色面で可読性を保ちます。 |
| サイズを柔軟にしたい | 一般的な比率、正確なピクセル、4モード、フォルダ一括に対応します。 |

## 写真を作品に変える流れ

```text
主題と関係を理解 → 輪郭・姿勢・方向・感情を抽出 → 二次情報を削除 → 粗いクレヨン線と少量のパステル面で再構成 → 淡い紙面と簡素な落書き記号に配置 → 余白と控えめな機械印字で仕上げる
```

## 完成品の識別ポイント

- 背景は明るく清潔なほぼ白い紙色で、主体の線と色面より明らかに明るい。
- 輪郭は太く、乾いた粉状で、途切れや揺れ、閉じきらない端部を含む。
- 周囲の記号は一筆か数筆の素朴な線で、精密なアイコンやステッカーにはしない。
- 主体は小さく、偏心、端寄せ、浮遊、部分切り取りなどになり、余白自体が構図を作る。
- 写真から親和性のある2–4色を抽出し、明るく柔らかなパステル色に整える。
- 文字は少量の編集的介入にとどめ、字間の揺らぎを持つ古い機械印字を使う。

## 4つの出力モード

- `top-bottom`：全幅の上下2領域のみ。実写を上、デザインを下に置き、各50%。
- `left-right`：全高の左右2領域のみ。実写を左、デザインを右に置き、各50%。上下構成へ回転しません。
- `design-only`：全画面を Panel 116 のデザイン翻訳にし、写真は見えない参照にします。
- `wallpaper-pack`：スマートフォン、iPad、デスクトップ、時計を端末ごとに生成。`linked` または `independent` を選べます。

モードと比率は複数指定できます。`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5`、正確なピクセルに対応します。文字はプロンプト生成、指定文の逐字使用、なしから選べます。フォルダ入力では各画像を分離して処理し、PNGを一つの新しいタスクフォルダへ置きます。

## はじめに

```bash
git clone https://github.com/nevertoday/xxd-panel-116.git
npx skills add https://github.com/nevertoday/xxd-panel-116 --skill xxd-panel-116
```

インストール後に Agent セッションを再起動し、`$xxd-panel-116` を呼び出します。ユーザー単位の Codex には `--global --agent codex --yes` を追加できます。

```text
/xxd-panel-116 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale ja-JP
/xxd-panel-116 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-116 photo.jpg --mode design-only --size 9:16 --text none
```

完全な実行契約は [SKILL.md](SKILL.md)、実行アダプターは[英語](references/xxd-panel-116-prompt.en.md)／[中国語](references/xxd-panel-116-prompt.zh-CN.md)を参照してください。

<!-- xxd-readme-ads:start -->
## XXD について

XXD は Xiaoxiaodong のブランド名略称です。本プロジェクトの作成・管理：[@xiaoxiaodong01](https://x.com/xiaoxiaodong01)。

## Xiaoxiaodong マルチプラットフォーム会員 · 年額 CNY 699

> **広告表示：** 以下のQRコード、会員および有料サービスのリンクはXXDの広告情報です。スキャンや購入は任意であり、オープンソースの利用には影響しません。

年額会員ひとつで、**Knowledge Planet＋XXD会員プロンプトライブラリ＋すべてのGeneral Skills会員**の3つを利用できます。別々に購入する必要はありません。

<!-- xxd-panel-command-system:start -->

### Skills の連携方法

| 区分 | 含まれるもの | 役割 |
|---|---|---|
| **General** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 利用可能な番号付きSkillsを検出し、画像・テーマ・用途から推薦し、複数スタイルや一括タスクを整理します。 |
| **Soldier** | `xxd-panel-NNN` | 各番号が固有の原文プロンプトと美学に従い、Generalから割り当てられた具体的な作業を完成させます。 |

<!-- xxd-panel-command-system:end -->

### 会員の内容

1. **XiaoxiaodongをAI学習の相談相手に**
   [Knowledge Planet](https://wx.zsxq.com/group/15554814142882)で、AI学習、ツール、実際のプロジェクトについていつでも質問できます。回答や役立つ内容を会員向けに整理していきます。
2. **継続更新する会員プロンプトライブラリ**
   [XXD会員プロンプトライブラリ](https://vip.xiaoxiaodong.ai/)には現在約3.2万件のプロンプトがあり、10万件超を目標に継続して拡充します。
3. **すべてのGeneral Skillsと利用サポート**
   ひとつの会員で全General Skillsを利用でき、使い方に困ったときは案内やQ&Aを受けられます。
4. **必要性の高い要望を優先**
   会員から寄せられた頻度と必要性の高いプロンプトやSkillsは、優先して検討・開発します。

### 開設方法

- [会員サイトから自分で開設](https://vip.xiaoxiaodong.ai/)できます。
- または下のQRコードからXiaoxiaodongに連絡し、開設を依頼できます。

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="Xiaoxiaodongへの連絡" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## ライセンス

本プロジェクト（Skill、プロンプト、スクリプト、文書、付属サンプル画像を含む）は **PolyForm Noncommercial License 1.0.0** の下で提供されます。完全な法的条文は [LICENSE](LICENSE)、公式ページは <https://polyformproject.org/licenses/noncommercial/1.0.0> を参照してください。

分かりやすく言うと：

- 個人は学習、研究、実験、テスト、趣味のプロジェクト、私的娯楽に使用できます。慈善団体、教育機関、公的研究・安全・保健機関、環境保護団体、政府機関も使用できます。
- **非商業目的**であれば、使用、複製、変更、派生物の作成、共有が可能です。共有時には本ライセンス（または上記リンク）と、作者が示したすべての `Required Notice:` 文を添付する必要があります。
- 商用製品・サービス、有料納品、アクセス権やライセンスの販売、商業利用につながることが予想される用途には使用できません。商用利用には著作権者から別途書面による許可を得てください。
- 本契約が付与するのは明記された著作権ライセンスと限定的な特許ライセンスだけです。商標、ブランド名、その他明記されていない権利は付与されず、ライセンスを第三者へ再許諾することもできません。
- 書面で違反通知を受けた場合、32 日以内に遵守状態へ戻り、実際の是正措置を取らなければライセンスは直ちに終了します。特許侵害を書面で主張した場合も特許ライセンスが終了します。
- 内容は法律が認める範囲で「現状のまま」提供され、保証はありません。利用に伴うリスクと損失は利用者が負います。
