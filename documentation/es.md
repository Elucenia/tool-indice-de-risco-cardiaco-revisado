<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · es · no clinical/professional/rights approval -->

# Índice de riesgo cardíaco revisado (Lee)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/indice-de-risco-cardiaco-revisado)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Cirugía de alto riesgo (intraperitoneal, intratorácica o vascular suprainguinal)

`cir`

### Cardiopatía isquémica (infarto previo, angina, prueba de isquemia positiva, uso de nitratos u onda Q en el ECG)

`dac`

### Insuficiencia cardíaca (antecedentes, edema pulmonar, disnea paroxística nocturna, tercer ruido o congestión en radiografía)

`icc`

### Enfermedad cerebrovascular (ictus o AIT)

`avc`

### Diabetes tratada con insulina

`insulina`

### Creatinina preoperatoria \> 2,0 mg/dL

`cr`

## Edición del método

RCRI/Lee 1999: 6 factores, total 0–6; sin recalibración automática

## Fórmula documentada

Un punto por factor: cirugía de alto riesgo, cardiopatía isquémica, insuficiencia cardíaca, enfermedad cerebrovascular, diabetes con insulina, creatinina \>2,0 mg/dL.

## Límites y población

El RCRI original se derivó en personas estables de al menos 50 años sometidas a cirugía no cardíaca mayor electiva. Las tasas son específicas de las cohortes históricas; no constituyen una calibración automática para cirugía urgente, otras poblaciones ni el hospital actual. Las definiciones de los factores y la interpretación deben seguir la guía vigente.

## Referencias

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
