<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · zh · no clinical/professional/rights approval -->

# 修订心脏风险指数（Lee）

[条件、来源与许可](https://elucenia.org/zh/tools/indice-de-risco-cardiaco-revisado)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 高风险手术（腹腔内、胸腔内或腹股沟以上血管手术）

`cir`

### 缺血性心脏病（既往心肌梗死、心绞痛、缺血试验阳性、使用硝酸酯或 ECG Q 波）

`dac`

### 心力衰竭（病史、肺水肿、阵发性夜间呼吸困难、第三心音或 X 线淤血）

`icc`

### 脑血管病（卒中或 TIA）

`avc`

### 使用胰岛素的糖尿病

`insulina`

### 术前肌酐 \> 2.0 mg/dL

`cr`

## 方法版本

RCRI/Lee 1999：6因素，总分0–6；无自动再校准

## 已记录的公式

每项1分：高风险手术、缺血性心脏病、心力衰竭、脑血管病、胰岛素治疗糖尿病、肌酐\>2.0 mg/dL。

## 限制与适用人群

原始RCRI在至少50岁、病情稳定且接受择期重大非心脏手术者中推导。发生率属于历史队列，并非对急诊手术、其他人群或当前医院的自动校准。因素定义和解释须结合现行指南。

## 参考文献

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

I级：0.4%的主要心脏并发症（Lee）；30天内死亡、心肌梗死或心肺复苏为3.9%（CCS 2017）


### 2

II至III级：按Lee队列为0.9%（1分）至6.6%（2分）；按CCS 2017为6.0%至10.1%

根据指南，考虑术前BNP/NT-proBNP和术后肌钙蛋白。


### 3

IV级：11%的主要心脏并发症（Lee）；30天内死亡、心肌梗死或心肺复苏为15%（CCS 2017）

高风险：心脏科评估、临床优化及术后肌钙蛋白监测。

