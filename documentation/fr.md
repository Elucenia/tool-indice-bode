<!-- ELUCENIA technical documentation · indice-bode · fr · no clinical/professional/rights approval -->

# Indice BODE

[conditions, sources et autorisations](https://elucenia.org/fr/outils/indice-bode)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### VEMS après bronchodilatateur

`vef1`

% de la valeur théorique · intervalle: 5–150

### Distance au test de marche de 6 minutes

`dist`

m · intervalle: 0–1000

### Dyspnée (échelle mMRC)

`mmrc`

- `0` — 0 : uniquement à l’effort intense
- `1` — 1 : en marchant vite ou en montant une côte
- `2` — 2 : marche plus lentement que les personnes du même âge ou s’arrête sur terrain plat
- `3` — 3 : s’arrête après ~100 m ou quelques minutes sur terrain plat
- `4` — 4 : ne sort pas de chez soi ou est essoufflé en s’habillant

### IMC

`imc`

kg/m² · intervalle: 10–70

## Édition de la méthode

BODE/Celli 2004 : IMC/VEMS/mMRC/6MWD, total 0–10 ; original, pas BODE actualisé

## Formule documentée

O (VEMS % prédit) : ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E (marche de 6 min) : ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B (IMC) : \> 21 = 0; ≤ 21 = 1.

## Limites et population

Le BODE original a été développé pour le pronostic de la BPCO à l’aide de mesures respiratoires et systémiques, dont la marche de six minutes. Il ne diagnostique pas la BPCO et ne fournit pas automatiquement une probabilité individuelle selon un horizon temporel ; les conditions du test, les définitions des items et l’éligibilité doivent correspondre à la version.

## Références

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
