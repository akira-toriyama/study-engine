---
version: alpha
name: study-engine Dark
description: >-
  Electron + React の SRS(SM-2)学習アプリ。落ち着いたダークテーマの上で、
  4 段階の学習グレード(Again / Hard / Good / Easy)と新規(New)を意味色で
  一貫表現する。色・タイポ・spacing は src/renderer/src/styles.css から抽出。
  角丸は実値(2–16px の幅)を代表 6 段に正規化(各 component は最も近い rung)。
colors:
  surface: "#0f1115"
  surface-panel: "#171a21"
  surface-panel2: "#1f2430"
  line: "#2a313f"
  on-surface: "#e6e9ef"
  muted: "#8b93a7"
  primary: "#5b8cff"
  good: "#3ecf8e"
  hard: "#e0b341"
  again: "#ef5f6b"
  easy: "#6fb1ff"
  new: "#b07cff"
  on-primary: "#ffffff"
  choice-picked: "#1d2740"
  choice-right: "#14322a"
  choice-wrong: "#34191e"
  hint-surface: "#222a18"
  hint-text: "#ece4c6"
  error-surface: "#3a1d22"
  error-text: "#ffd7da"
  explanation-text: "#cfd5e2"
  grade1-surface: "#34191e"
  grade2-surface: "#2c2613"
  grade3-surface: "#14322a"
  grade4-surface: "#16263f"
  heat-l0: "#1d2430"
  heat-l1: "#1f4d37"
  heat-l2: "#2a7d52"
  heat-l3: "#34b06f"
  heat-l4: "#3ecf8e"
typography:
  h1:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.6
  brand:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 17px
    fontWeight: 800
    lineHeight: 1.6
  hero-score:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 56px
    fontWeight: 800
    lineHeight: 1.1
  stat-num:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 24px
    fontWeight: 800
    lineHeight: 1.6
  question-body:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.6
  body-md:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
  label-sm:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.6
  caption-xs:
    fontFamily: -apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.6
  mono:
    fontFamily: ui-monospace, SFMono-Regular, Menlo, monospace
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.6
rounded:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 12px
  xl: 16px
  full: 999px
spacing:
  xxs: 2px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 24px
  xxl: 28px
  card-padding: 26px
  page-max: 1120px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 12px 20px
  button-primary-redrill:
    backgroundColor: "{colors.again}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
  button-ghost:
    backgroundColor: transparent
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 11px 16px
  card:
    backgroundColor: "{colors.surface-panel}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.xl}"
    padding: "{spacing.card-padding}"
  question-body:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    typography: "{typography.question-body}"
    rounded: "{rounded.md}"
    padding: 16px 20px
  choice:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 16px 18px
  choice-picked:
    backgroundColor: "{colors.choice-picked}"
  choice-right:
    backgroundColor: "{colors.choice-right}"
  choice-wrong:
    backgroundColor: "{colors.choice-wrong}"
  pill:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 3px 9px
  pill-new:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.new}"
    rounded: "{rounded.full}"
  pill-due:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.easy}"
    rounded: "{rounded.full}"
  input:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    padding: 5px 8px
  answer-input:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 13px 16px
  grade-good:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.good}"
  grade-hard:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.hard}"
  grade-again:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.again}"
  grade-easy:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.easy}"
  chat-msg-user:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 8px 12px
  chat-msg-assistant:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 8px 12px
  toast:
    backgroundColor: "{colors.surface-panel2}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 10px 18px
  divider:
    backgroundColor: "{colors.line}"
  caption:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
  hint-box:
    backgroundColor: "{colors.hint-surface}"
    textColor: "{colors.hint-text}"
    rounded: "{rounded.md}"
    padding: 12px 16px
  error-box:
    backgroundColor: "{colors.error-surface}"
    textColor: "{colors.error-text}"
    rounded: "{rounded.md}"
    padding: 10px 14px
  explanation:
    backgroundColor: "{colors.surface-panel}"
    textColor: "{colors.explanation-text}"
  grade-chip-1:
    backgroundColor: "{colors.grade1-surface}"
    textColor: "{colors.again}"
    rounded: "{rounded.sm}"
    padding: 3px 9px
  grade-chip-2:
    backgroundColor: "{colors.grade2-surface}"
    textColor: "{colors.hard}"
    rounded: "{rounded.sm}"
  grade-chip-3:
    backgroundColor: "{colors.grade3-surface}"
    textColor: "{colors.good}"
    rounded: "{rounded.sm}"
  grade-chip-4:
    backgroundColor: "{colors.grade4-surface}"
    textColor: "{colors.easy}"
    rounded: "{rounded.sm}"
  heatmap-cell-l0:
    backgroundColor: "{colors.heat-l0}"
    rounded: "{rounded.xs}"
  heatmap-cell-l1:
    backgroundColor: "{colors.heat-l1}"
    rounded: "{rounded.xs}"
  heatmap-cell-l2:
    backgroundColor: "{colors.heat-l2}"
    rounded: "{rounded.xs}"
  heatmap-cell-l3:
    backgroundColor: "{colors.heat-l3}"
    rounded: "{rounded.xs}"
  heatmap-cell-l4:
    backgroundColor: "{colors.heat-l4}"
    rounded: "{rounded.xs}"
---

# study-engine Dark — DESIGN.md

> このファイルは study-engine の **既存の見た目を写し取った** spec(新しいデザインの
> 発明ではない)。色・タイポ・spacing は `src/renderer/src/styles.css` から抽出し、
> 角丸だけは実値(2–16px の幅)を代表 6 段に正規化している(各 component は最も近い
> rung)。値を変えたいときは styles.css と本ファイルを同一 PR で更新する。

## Overview

study-engine は Electron + React + TypeScript の SRS(間隔反復・SM-2)学習アプリ。
ダッシュボードでドメインを選び、1 問ずつ出題ラリーをこなして 4 段階で自己評価する
「出題ラリー UI」が中核体験。長時間の学習でも目が疲れない**落ち着いたダークテーマ**を
基調とし、画面は静かで情報密度は中程度。色は飾りではなく**意味**を運ぶ:
学習グレード(Again / Hard / Good / Easy)と新規(New)に固定の意味色を割り当て、
グレードバー・選択肢の正誤・結果一覧・ヒートマップまで同じ色語彙で貫く。

トーンは「集中を妨げない・自己評価を素早く下せる」。アクセント青(primary)は
1 画面につき「最も重要な 1 アクション」(出題開始・送信・進捗バー)に限って使い、
意味色はグレード判定にだけ使うことで、色のノイズを避け判断を速くする。

## Colors

パレットは**暗い neutral 4 階層** + **単一のアクセント青** + **5 つの学習意味色**で構成。

- **Surface (#0f1115):** アプリ最背面。最も暗い地。topbar は同色の半透明
  (`rgba(15,17,21,0.9)`)+ blur で重ねる。
- **Surface Panel (#171a21):** カード・モーダル・チャットパネル・統計ピルなど
  「1 段持ち上げた面」。
- **Surface Panel2 (#1f2430):** 入力欄・選択肢・コードチップ・ツールチップなど
  「面の中のへこみ/コントロール」。
- **Line (#2a313f):** 区切り線とボーダーの既定色。フラットデザインの階層は影でなく
  この線とトーン差で表す(§Elevation)。
- **On-surface (#e6e9ef):** 本文の主要テキスト色。
- **Muted (#8b93a7):** メタ情報・ラベル・補助テキスト・無効寄りの説明。

アクセントと学習意味色:

- **Primary (#5b8cff):** 唯一のアクション色。主ボタン・進捗バー・question-body の
  左 3px ボーダー・hover 時のボーダー強調・統計の数値に使う。「やり直し(redrill)」
  ボタンだけは赤(again)で primary を上書きし「間違えた分を反復する」意味を出す。
- **Good (#3ecf8e / grade 3):** 正解・成熟・ヒートマップ最濃。
- **Hard (#e0b341 / grade 2):** 難・ヒント枠・leech(つまずき)フラグ。
- **Again (#ef5f6b / grade 1):** 不正解・エラー枠・cram の取りこぼし。
- **Easy (#6fb1ff / grade 4):** 容易・due(復習期限)ピル・cloze の空欄ハイライト・
  リンク色・出典チップ・読み上げボタン。
- **New (#b07cff):** 新規問題。新規ピル・新規カウントの数値。

背景付き状態色(選択肢の正誤・結果グレードチップ・エラー/ヒント枠)は、上の意味色を
前景に、対応する**暗い同系色**を背景に置く(例: 正解 `#14322a` 地に good 文字、
不正解 `#34191e` 地に again 文字)。grade チップ g1〜g4 と choice の right/wrong、
result-row の左ボーダーまで同じ対応で揃える。

ヒートマップ(GitHub 風の学習量グリッド)は緑の 5 段(`#1d2430`→`#1f4d37`→
`#2a7d52`→`#34b06f`→good)。これは good を頂点とする独立スケールで、意味色の good に
連続させてある。

## Typography

フォントは macOS のシステムフォント前提の単一スタックで、日本語問題を素直に表示する:
`-apple-system, BlinkMacSystemFont, 'Hiragino Sans', 'Noto Sans JP', sans-serif`。
別ファミリは導入せず、**サイズと太さ**だけで階層を作る。等幅(`ui-monospace,
SFMono-Regular, Menlo, monospace`)は ID ピルとインラインコード/コードブロックに限定。

- **Body (15px / 400 / line-height 1.6):** `body` の既定。日本語の可読性のため
  行間はやや広め。
- **H1 (22px / 700):** 画面見出し。
- **Brand (17px / 800):** topbar のアプリ名。最も太い 800 を識別子として使う。
- **Question Body (20px / 600):** 出題本文。`--q-size` 変数が起点で、設定の
  `fontSize` から上書きできる(学習者が読みやすさを調整)。選択肢/記述入力は
  `calc(var(--q-size) - 4px)` なので token も question-body 基準で読む。
- **Hero Score (56px / 800):** 結果画面の正答率。画面で一番大きい数字。
- **Stat Num (24px / 800):** ダッシュボードの統計ピルの数値。
- **Label / Caption (13px / 12px / 11px, 400):** メタ・ピル・凡例・出典。muted と
  併用。最小の 11px は出典チップ・凡例・ヒートマップ補助など。
- **Mono (10px):** ID ピル。コードチップ/ブロックはこの monospace ファミリを継ぐ。

## Layout

中央寄せの**固定最大幅**レイアウト。ダッシュボードとセッションは `max-width: 1120px`
で中央寄せ、チャットを開いたセッションだけ `1500px` に広げて 2 カラム(左=出題、
右=`360px` 固定のチャットパネル sticky)にする。

spacing は厳密な 4px の倍数を基本リズムにする(`4 / 8 / 12 / 18 / 24 / 28`)。
カードの内側余白は広め(26px)で、密度より落ち着きを優先。ページ下端には
大きめの余白(`padding-bottom: 60px`)を取り、アクションが画面端に貼り付かないようにする。
ドメイン一覧は `repeat(auto-fill, minmax(240px, 1fr))` のグリッド、統計・グレードバーは
flex + `flex-wrap` で、ラベルを途中改行させずに行ごと折り返す。

## Elevation & Depth

影は控えめ。階層は基本的に**トーンの差(surface → panel → panel2)とボーダー
(line)**で表現するフラット寄りの設計。影を使うのは「浮く」要素に限定する:

- モーダルカード: `0 12px 40px rgba(0,0,0,0.6)`(backdrop は `rgba(0,0,0,0.55)`)。
- ツールチップ pop: `0 8px 26px rgba(0,0,0,0.5)`。
- トースト: `0 6px 24px rgba(0,0,0,0.4)`。

topbar は `position: sticky` + 半透明地 + `backdrop-filter: blur(8px)` で、
スクロール内容の上に薄く重なる擬似的な奥行きを出す。question-body は左 3px の
primary ボーダー、結果行は左 3px の good/again ボーダーで「色のアクセントによる
持ち上げ」を作る。

## Shapes

角丸は用途ごとに段階を持つ。小さなコントロールほど小さい半径:

- **xs 2px:** ヒートマップのセル。
- **sm 6px:** 小さな select・出典/コードチップ系の小コントロール(実値 5–7px)。
- **md 10px:** ボタン・トースト・ヒント枠・エラー枠・question-body(実値 10–11px)。
- **lg 12px:** 選択肢・チャット吹き出し・記述入力(実値 11–12px)。
- **xl 16px:** メインカード・チャットパネル・モーダル(実値 14–16px)。
- **full 999px:** ピル(`border-radius: 999px`)と丸アイコン(`50%`)。

> 注: 実 CSS の border-radius は 2–16px に細かく分布(2/5/6/8/10/11/12/14/16px)。
> ここでは代表 6 段に正規化し、各 component は最も近い rung を指す(±1–2px の丸めあり)。
> 色・タイポ・spacing は実値そのまま。

シャープな角は使わず、全面的に丸角で統一して柔らかい印象にする。

## Components

- **Buttons:** `primary` はアクセント青地に白文字、`10px` 角・`12px 20px`。無効時は
  `opacity: 0.4`。`redrill` バリアントは again 赤地。`ghost-btn` は透明地 +
  line ボーダー。`link` は枠なしの muted テキストボタン。
- **Choice(選択肢):** panel2 地・line ボーダー・`12px` 角。hover で primary ボーダー +
  `translateY(-1px)`。状態は `picked`(青地 #1d2740)/ `right`(緑地 #14322a)/
  `wrong`(赤地 #34191e)。
- **Pill / Chip:** panel2 地・`999px`・11px。`new` は new 色の文字+ボーダー、
  `due` は easy 色。`id-pill` は monospace 10px・muted。
- **Grade buttons(4 段階):** 既定は panel2 地・muted 寄り。hover で各グレード色に
  ボーダーが点灯(again/hard/good/easy)。`suggested`(自動採点の推奨)は primary の
  `outline` で示す。
- **Input / Textarea:** panel2 地・line ボーダー。小入力は `6px` 角、回答記述
  (`answer-input`)は `12px`(実 11px)角・`min-height: 110px`・`resize: vertical`。
- **Chat message:** user は primary 青地に白(右寄せ)、assistant は panel2 地 +
  line ボーダー(左寄せ)。パネルは `360px` 固定・sticky・`16px` 角。
- **Tooltip(infotip):** panel2 地・`10px` 角・`260px` 上限。トリガーの ⓘ は
  hover で primary 色。6px の隙間を透明ブリッジで埋めて hover が途切れないようにする。
- **Toast:** panel2 地・primary ボーダー・画面下中央固定。

## Do's and Don'ts

- Do: アクセント青(primary)は 1 画面の最重要アクション(出題開始・送信・進捗)に
  限って使う。意味色はグレード判定にだけ使う。
- Do: 学習グレードの色対応を固定する — Again=赤 / Hard=黄 / Good=緑 / Easy=青系 /
  New=紫。グレードバー・選択肢・結果一覧・チップで必ず同じ色に揃える。
- Do: 階層はトーン差(surface→panel→panel2)とボーダー(line)で出す。影は
  モーダル・ツールチップ・トーストなど「浮く」要素だけ。
- Do: 角はすべて丸角で統一する(コントロールほど小さい半径)。
- Don't: 学習意味色を装飾目的で乱用しない(色のノイズが自己評価の判断を遅らせる)。
- Don't: 別フォントファミリを増やさない。階層はサイズと太さで作る(等幅は ID と
  コードのみ)。
- Don't: question-body のサイズを固定値で直書きしない。`--q-size` 変数(設定で可変)を
  起点にし、選択肢/入力は `calc(var(--q-size) - 4px)` で追従させる。
- Don't: シャープな角と丸角を同一ビューで混ぜない。
- Note(コントラスト): アクセント青(primary)/again 赤の上の白文字は WCAG AA(4.5:1)
  未満(3.16–3.22:1)。ブランドのアクセント/意味色として意図的に許容しているが、
  本文テキストには使わない(主要テキストは on-surface #e6e9ef)。