<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · ja · no clinical/professional/rights approval -->

# PaO₂/FiO₂比・ARDS（Berlin定義）

[条件・出典・許諾](https://elucenia.org/ja/tools/relacao-pao2-fio2)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### PaO₂

`pao2`

mmHg · 範囲: 20–700

### FiO₂

`fio2`

% · 範囲: 21–100

### PEEP または CPAP

`peep`

cmH₂O · 任意 · 範囲: 0–30

### SpO₂（SpO₂/FiO₂比用）

`spo2`

% · 任意 · 範囲: 50–100

## 方法の版

Berlin ARDS 2012：P/F 100/200/300+PEEP/文脈、Global Definition 2024のS/F、SpO₂≤97

## 記載された計算式

P/F比 = PaO₂ (mmHg) ÷ FiO₂ (割合: 40% = 0.40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (割合), 解釈可能条件 SpO₂ ≤ 97%.

## 限界・対象集団

P/F比は、急性呼吸窮迫症候群（ARDS）の定義の一要素にすぎません。Berlin分類には、酸素化の閾値に加えて最終定義の他の条件が必要で、比だけではARDSは確定しません。S/Fによる分類は後のグローバル定義に属し、Berlinの草案から削除された補助変数を混在させず、専用の基準を用いる必要があります。

## 参考文献

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

300を超える比：ARDSの酸素化基準なし


### 2

ベルリン基準による軽症ARDS（200～300）

酸素化は基準の1つにすぎません：1週間以内の発症、両側性陰影、心不全または循環血液量増加では説明できない浮腫。


### 3

ベルリン基準による中等症ARDS（100～200）

酸素化は基準の1つにすぎません：1週間以内の発症、両側性陰影、心不全または循環血液量増加では説明できない浮腫。


### 4

ベルリン基準による重症ARDS（≤ 100）

| 結果の詳細 | |
| --- | --- |
| SpO₂/FiO₂ | 113（≤ 315：2023年のグローバル定義における低酸素血症基準） |

酸素化は基準の1つにすぎません：1週間以内の発症、両側性陰影、心不全または循環血液量増加では説明できない浮腫。

