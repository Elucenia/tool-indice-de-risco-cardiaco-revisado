<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · ja · no clinical/professional/rights approval -->

# 改訂心臓リスク指数（Lee）

[条件・出典・許諾](https://elucenia.org/ja/tools/indice-de-risco-cardiaco-revisado)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 高リスク手術（腹腔内、胸腔内、鼠径部より上の血管手術）

`cir`

### 虚血性心疾患（心筋梗塞既往、狭心症、虚血検査陽性、硝酸薬、ECGのQ波）

`dac`

### 心不全（既往、肺水腫、発作性夜間呼吸困難、S3、X線うっ血）

`icc`

### 脳血管疾患（脳卒中またはTIA）

`avc`

### インスリン使用中の糖尿病

`insulina`

### 術前クレアチニン \> 2.0 mg/dL

`cr`

## 方法の版

RCRI/Lee 1999：6因子、計0–6；自動再校正なし

## 記載された計算式

因子ごと1点：高リスク手術、虚血性心疾患、心不全、脳血管疾患、インスリン治療糖尿病、クレアチニン\>2.0 mg/dL。

## 限界・対象集団

原RCRIは、少なくとも50歳の安定した人で、予定された大規模な非心臓手術を受ける対象から導出されました。率は歴史的コホートに固有であり、緊急手術、他の集団、現在の病院に自動的に較正されたものではありません。因子の定義と解釈は、現行のガイドラインに従う必要があります。

## 参考文献

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

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

クラスI：主要心臓合併症 0.4%（Lee）；30日以内の死亡、MI、またはCPR 3.9%（CCS 2017）


### 2

クラスII～III：Leeコホートでは0.9%（1点）～6.6%（2点）；CCS 2017では6.0%～10.1%

ガイドラインに従い、術前BNP/NT-proBNPおよび術後トロポニンを考慮する。


### 3

クラスIV：主要心臓合併症 11%（Lee）；30日以内の死亡、MI、またはCPR 15%（CCS 2017）

高リスク：循環器評価、臨床的最適化、ならびにトロポニンによる術後監視。

