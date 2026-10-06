<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · de · no clinical/professional/rights approval -->

# Revidierter kardialer Risikoindex (Lee)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/indice-de-risco-cardiaco-revisado)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Hochrisikooperation (intraperitoneal, intrathorakal oder suprainguinal vaskulär)

`cir`

### Ischämische Herzerkrankung (früherer Myokardinfarkt, Angina pectoris, positiver Ischämietest, Nitrateinnahme oder Q-Zacke im EKG)

`dac`

### Herzinsuffizienz (Anamnese, Lungenödem, paroxysmale nächtliche Dyspnoe, dritter Herzton oder Röntgenstauung)

`icc`

### Zerebrovaskuläre Erkrankung (Schlaganfall oder TIA)

`avc`

### Insulinbehandelter Diabetes

`insulina`

### Präoperatives Kreatinin \> 2,0 mg/dL

`cr`

## Fassung der Methode

RCRI/Lee 1999: 6 Faktoren, gesamt 0–6; keine automatische Rekalibrierung

## Dokumentierte Formel

Ein Punkt je Faktor: Hochrisikooperation, ischämische Herzkrankheit, Herzinsuffizienz, zerebrovaskuläre Krankheit, insulinbehandelter Diabetes, Kreatinin \>2,0 mg/dL.

## Grenzen und Population

Der ursprüngliche RCRI wurde bei stabilen Personen ab 50 Jahren mit großer elektiver nichtkardialer Operation entwickelt. Die Raten sind spezifisch für historische Kohorten; sie sind keine automatische Kalibrierung für dringliche Operationen, andere Populationen oder das heutige Krankenhaus. Faktorendefinitionen und Interpretation müssen die geltende Leitlinie berücksichtigen.

## Referenzen

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Klasse I: 0,4 % schwere kardiale Komplikationen (Lee); 3,9 % Tod, MI oder CPR innerhalb von 30 Tagen (CCS 2017)


### 2

Klasse II bis III: 0,9 % (1 Punkt) bis 6,6 % (2 Punkte) in der Lee-Kohorte; 6,0 % bis 10,1 % nach CCS 2017

Präoperatives BNP/NT-proBNP und postoperative Troponinbestimmung gemäß der Leitlinie in Betracht ziehen.


### 3

Klasse IV: 11 % schwere kardiale Komplikationen (Lee); 15 % Tod, MI oder CPR innerhalb von 30 Tagen (CCS 2017)

Hohes Risiko: kardiologische Beurteilung, klinische Optimierung und postoperative Überwachung mit Troponin.

