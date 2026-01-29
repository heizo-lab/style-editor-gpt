Style Editor GPT





概要



Style Editor GPT は、文章の内容には介入せず、文体・表現・癖の一貫性だけを守るための編集支援 GPT です。
本 GPT は「文章を書く存在」ではなく、「書き手の文体を壊さずに整える番人」として設計されています。

- 代筆しない
- 主張を変えない
- 意味を補完しない
- 文体と表現の揺れのみを扱う


長文・複数人執筆・仕様書・論考など、
「誰が書いたか」より 「どう書かれているか」 が重要な文章に向いています。

---



この GPT がやらないこと（重要）



- 新しい表現の提案
- 文学的・AI的な言い換え
- 語彙の高度化
- 内容の正誤判断
- 思想・立場・結論への介入


👉 意味に踏み込まないこと自体が、この GPT の設計思想です。

---



設計思想（Constitution-based Design）



Style Editor GPT は、
「スタイルエディター憲法（constitution）」を最上位ルールとして動作します。

この憲法は、

- 編集者としての役割を厳密に定義し
- 判断してよいこと／してはいけないことを明確にし
- 「判断保留」という行為を正当な編集行為として認める


ためのものです。

GPT が 便利さの名のもとに踏み込みすぎることを防ぐ ため、
あえて強い制約を与えています。

---



ディレクトリ構造


```
style-editor-gpt/
├─ constitution/
│  └─ style_editor_constitution.md
│
├─ rules/
│  ├─ style_guide.md
│  ├─ style_checklist.md
│  └─ usage_rules.md
│
├─ interviews/
│  ├─ onboarding_interview.md
│  └─ initial_interview.md
│
├─ terminology/
│  └─ terminology.md
│
├─ references/
│  └─ reference_text.md
│
├─ examples/
│  └─ before_after_sample.md
│
├─ drafts/
│  └─ notes.md
│
└─ README.md
```

---



各ファイルの役割





constitution/



- style_editor_constitution.md
  この GPT の最上位ルール。
  役割・禁止事項・判断保留ルール・出力形式を定義します。


---



rules/



- style_guide.md
  文末・接続詞・推量表現など、案件ごとに差し替え可能な文体ルール。
- style_checklist.md
  編集後のセルフチェック用リスト。
- usage_rules.md
  GPT の使い方・入力方法・注意点。


---



interviews/



- onboarding_interview.md
  作業を開始してよいか判断するための簡易ヒアリング。
- initial_interview.md
  文体・用途・制約条件を確定するための詳細ヒアリング。


---



terminology/



- terminology.md
  意味の定義ではなく、誤変換・誤認識を防ぐための編集補助用語集。
  専門用語や内部用語の扱いを安定させる目的で使用します。


---



references/



- reference_text.md
  文体判断の参考資料。
  模倣は禁止されており、あくまで判断補助としてのみ使用します。


---



examples/



- before_after_sample.md
  修正前／修正後の比較例。
  「どこまで直すか」の感覚共有用。


---



drafts/



- notes.md
  思考メモ・試行錯誤・未整理のルールを置く場所。


---



想定ユースケース



- 5万字以上の長文編集
- 複数人執筆の原稿統一
- 仕様書・論考・レポート
- 「AIっぽさを消したい」文章編集
- GPT を編集者として使いたいケース


---



ライセンス



This project is released under the MIT License.
You are free to use, modify, and adapt it for your own GPTs or editorial workflows.

---



注意事項



- 本リポジトリは 「文章を書く GPT」ではありません
- 出力内容の最終判断は必ず人間が行ってください
- 憲法とルールの解釈に迷った場合は、判断を保留することが正解です


## 使い方（概要）
1. onboarding_interview.md に回答
2. initial_interview.md で条件確定
3. 本文を投入
4. 出力フォーマットに従って提案を受け取る
---