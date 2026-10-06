<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · it · no clinical/professional/rights approval -->

# Indice di rischio cardiaco rivisto (Lee)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/indice-de-risco-cardiaco-revisado)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Chirurgia ad alto rischio (intraperitoneale, intratoracica o vascolare soprainguinale)

`cir`

### Cardiopatia ischemica (infarto pregresso, angina, test di ischemia positivo, uso di nitrati o onda Q all’ECG)

`dac`

### Insufficienza cardiaca (anamnesi, edema polmonare, dispnea parossistica notturna, terzo tono o congestione radiografica)

`icc`

### Malattia cerebrovascolare (ictus o TIA)

`avc`

### Diabete trattato con insulina

`insulina`

### Creatinina preoperatoria \> 2,0 mg/dL

`cr`

## Edizione del metodo

RCRI/Lee 1999: 6 fattori, totale 0–6; nessuna ricalibrazione automatica

## Formula documentata

Un punto per fattore: chirurgia ad alto rischio, cardiopatia ischemica, scompenso, malattia cerebrovascolare, diabete con insulina, creatinina \>2,0 mg/dL.

## Limiti e popolazione

L’RCRI originale è stato derivato in persone stabili di almeno 50 anni sottoposte a chirurgia maggiore elettiva non cardiaca. I tassi sono specifici delle coorti storiche; non costituiscono una calibrazione automatica per chirurgia urgente, altre popolazioni o l’ospedale attuale. Definizioni dei fattori e interpretazione devono seguire la linea guida vigente.

## Riferimenti

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Classe I: 0,4% di complicanze cardiache maggiori (Lee); 3,9% di morte, IM o RCP entro 30 giorni (CCS 2017)


### 2

Classe II a III: dallo 0,9% (1 punto) al 6,6% (2 punti) nella coorte di Lee; dal 6,0% al 10,1% secondo CCS 2017

Considerare BNP/NT-proBNP preoperatorio e troponina postoperatoria, secondo la linea guida.


### 3

Classe IV: 11% di complicanze cardiache maggiori (Lee); 15% di morte, IM o RCP entro 30 giorni (CCS 2017)

Alto rischio: valutazione cardiologica, ottimizzazione clinica e sorveglianza postoperatoria con troponina.

