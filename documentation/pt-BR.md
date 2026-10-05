<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · pt-BR · no clinical/professional/rights approval -->

# Índice de Risco Cardíaco Revisado (Lee)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/indice-de-risco-cardiaco-revisado)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Cirurgia de alto risco (intraperitoneal, intratorácica ou vascular suprainguinal)

`cir`

### Doença isquêmica do coração (IAM prévio, angina, teste de isquemia positivo, uso de nitrato ou onda Q no ECG)

`dac`

### Insuficiência cardíaca (história, edema pulmonar, dispneia paroxística noturna, B3 ou congestão na radiografia)

`icc`

### Doença cerebrovascular (AVC ou AIT)

`avc`

### Diabetes em uso de insulina

`insulina`

### Creatinina pré-operatória \> 2,0 mg/dL

`cr`

## Edição do método

RCRI/Lee 1999:6 fatores, total 0–6; sem recalibração automática

## Fórmula documentada

Um ponto para cada fator: cirurgia de alto risco, doença isquêmica do coração, insuficiência cardíaca, doença cerebrovascular, diabetes com insulina e creatinina \> 2,0 mg/dL.

## Limites e população

O RCRI original foi derivado em pessoas estáveis de pelo menos 50 anos submetidas a cirurgia não cardíaca eletiva de grande porte. As taxas são específicas das coortes históricas; não constituem calibração automática para cirurgia urgente, outras populações ou hospital atual. Definições de fatores e interpretação devem acompanhar a diretriz vigente.

## Referências

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
