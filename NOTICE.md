# ライセンス表記

## general_dict.js（汎用言い換え辞書）

SudachiDict の同義語辞書（synonyms.txt）を変換して生成したものです。

- 出典: https://github.com/WorksApplications/SudachiDict
- ライセンス: Apache License 2.0
- Copyright (c) Works Applications Co., Ltd.

変換内容: グループID単位で語をまとめ、展開制御フラグ=2（展開禁止）の行を除外し、2語以上のグループのみをJS配列化（26,036グループ・70,148語）。

再生成する場合:
1. synonyms.txt を上記リポジトリ（src/main/text/synonyms.txt）から取得
2. グループID（1列目）でまとめ、9列目の語を収集（3列目=2はスキップ）
3. `const GENERAL_DICT=[[...],...]` 形式で general_dict.js に出力

## index.html 内の創作向け手作り辞書（DICT）

Mimilyオリジナル。約70項目・創作頻出語（動作・副詞・感情・身体反応・形容）に特化。
