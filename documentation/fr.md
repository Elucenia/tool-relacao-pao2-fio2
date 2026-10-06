<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · fr · no clinical/professional/rights approval -->

# Rapport PaO₂/FiO₂ et SDRA (Berlin)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/relacao-pao2-fio2)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### PaO₂

`pao2`

mmHg · intervalle: 20–700

### FiO₂

`fio2`

% · intervalle: 21–100

### PEEP ou CPAP

`peep`

cmH₂O · facultatif · intervalle: 0–30

### SpO₂ (pour le rapport SpO₂/FiO₂)

`spo2`

% · facultatif · intervalle: 50–100

## Édition de la méthode

Berlin SDRA 2012 : P/F 100/200/300+PEEP/contexte ; S/F de définition globale 2024, SpO₂≤97

## Formule documentée

Rapport P/F = PaO₂ (mmHg) ÷ FiO₂ (fraction: 40% = 0,40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (fraction), interprétable si SpO₂ ≤ 97%.

## Limites et population

Le rapport P/F n’est qu’un composant de la définition du SDRA. La classification de Berlin exige les autres conditions de la définition finale, en plus des limites d’oxygénation ; le rapport seul ne confirme pas un SDRA. La classification par S/F appartient à la définition mondiale ultérieure et exige ses propres critères, sans mélanger les variables auxiliaires retirées du projet de Berlin.

## Références

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

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

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Rapport supérieur à 300 : pas de critère d’oxygénation pour le SDRA


### 2

SDRA léger selon le critère de Berlin (200 à 300)

L’oxygénation n’est qu’un des critères : début en moins d’1 semaine, opacités bilatérales et œdème non expliqué par une insuffisance cardiaque ou une hypervolémie.


### 3

SDRA modéré selon le critère de Berlin (100 à 200)

L’oxygénation n’est qu’un des critères : début en moins d’1 semaine, opacités bilatérales et œdème non expliqué par une insuffisance cardiaque ou une hypervolémie.


### 4

SDRA sévère selon le critère de Berlin (≤ 100)

| Détails du résultat | |
| --- | --- |
| SpO₂/FiO₂ | 113 (≤ 315 : critère d’hypoxémie de la définition globale de 2023) |

L’oxygénation n’est qu’un des critères : début en moins d’1 semaine, opacités bilatérales et œdème non expliqué par une insuffisance cardiaque ou une hypervolémie.

