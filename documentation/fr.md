<!-- ELUCENIA technical documentation · indice-de-risco-cardiaco-revisado · fr · no clinical/professional/rights approval -->

# Indice de risque cardiaque révisé (Lee)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/indice-de-risco-cardiaco-revisado)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Chirurgie à haut risque (intrapéritonéale, intrathoracique ou vasculaire supra-inguinale)

`cir`

### Cardiopathie ischémique (infarctus antérieur, angor, test d’ischémie positif, prise de nitrés ou onde Q à l’ECG)

`dac`

### Insuffisance cardiaque (antécédent, œdème pulmonaire, dyspnée paroxystique nocturne, troisième bruit ou congestion radiographique)

`icc`

### Maladie cérébrovasculaire (AVC ou AIT)

`avc`

### Diabète traité par insuline

`insulina`

### Créatinine préopératoire \> 2,0 mg/dL

`cr`

## Édition de la méthode

RCRI/Lee 1999 : 6 facteurs, total 0–6 ; sans recalibrage automatique

## Formule documentée

Un point par facteur : chirurgie à haut risque, cardiopathie ischémique, insuffisance cardiaque, maladie cérébrovasculaire, diabète sous insuline, créatinine \>2,0 mg/dL.

## Limites et population

Le RCRI original a été développé chez des personnes stables d’au moins 50 ans subissant une chirurgie non cardiaque majeure programmée. Les taux sont propres aux cohortes historiques ; ils ne constituent pas un calibrage automatique pour la chirurgie urgente, d’autres populations ou l’hôpital actuel. Les définitions des facteurs et l’interprétation doivent accompagner la recommandation en vigueur.

## Références

- [Lee TH et al. Derivation and prospective validation of a simple index for prediction of cardiac risk of major noncardiac surgery. Circulation, 1999.](https://doi.org/10.1161/01.CIR.100.10.1043)

- [Duceppe E et al. Canadian Cardiovascular Society guidelines on perioperative cardiac risk assessment and management for patients who undergo noncardiac surgery. Can J Cardiol, 2017.](https://doi.org/10.1016/j.cjca.2016.09.008)

- [Halvorsen S et al. 2022 ESC Guidelines on cardiovascular assessment and management of patients undergoing non-cardiac surgery. Eur Heart J, 2022.](https://doi.org/10.1093/eurheartj/ehac270)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
