<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · en · no clinical/professional/rights approval -->

# Revised Cardiac Risk Index (Lee)

[conditions, sources and permissions](https://elucenia.org/en/tools/indice-de-risco-cardiaco-revisado)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### High-risk surgery (intraperitoneal, intrathoracic or suprainguinal vascular)

`cir`

### Ischemic heart disease (previous myocardial infarction, angina, positive ischemia test, nitrate use or Q wave on ECG)

`dac`

### Heart failure (history, pulmonary edema, paroxysmal nocturnal dyspnea, S3 or congestion on radiograph)

`icc`

### Cerebrovascular disease (stroke or TIA)

`avc`

### Insulin-treated diabetes

`insulina`

### Preoperative creatinine \> 2.0 mg/dL

`cr`

## Method edition

RCRI/Lee 1999: 6 factors, total 0–6; no automatic recalibration

## Documented formula

One point per factor: high-risk surgery, ischaemic heart disease, heart failure, cerebrovascular disease, insulin-treated diabetes and creatinine \>2.0 mg/dL.

## Limits and population

The original RCRI was derived in stable people aged at least 50 years undergoing major elective noncardiac surgery. Rates are specific to the historical cohorts; they do not automatically calibrate for urgent surgery, other populations or the current hospital. Factor definitions and interpretation must follow the current guideline.

## References

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Class I: 0.4% major cardiac complications (Lee); 3.9% death, MI or CPR in 30 days (CCS 2017)


### 2

Class II to III: 0.9% (1 point) to 6.6% (2 points) by the Lee cohort; 6.0% to 10.1% by CCS 2017

Consider preoperative BNP/NT-proBNP and postoperative troponin, as per the guideline.


### 3

Class IV: 11% major cardiac complications (Lee); 15% death, MI or CPR in 30 days (CCS 2017)

High risk: cardiology evaluation, clinical optimization and postoperative troponin monitoring.

