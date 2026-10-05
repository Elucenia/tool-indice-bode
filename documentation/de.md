<!-- ELUCENIA technical documentation · indice-bode · de · no clinical/professional/rights approval -->

# BODE-Index

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/indice-bode)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### FEV₁ nach Bronchodilatation

`vef1`

% des Sollwerts · Bereich: 5–150

### Strecke im 6-Minuten-Gehtest

`dist`

m · Bereich: 0–1000

### Dyspnoe (mMRC-Skala)

`mmrc`

- `0` — 0: nur bei starker Belastung
- `1` — 1: bei schnellem Gehen oder bergauf
- `2` — 2: geht langsamer als Gleichaltrige oder bleibt beim Gehen auf ebener Strecke stehen
- `3` — 3: bleibt nach ~100 m oder wenigen Minuten auf ebener Strecke stehen
- `4` — 4: verlässt das Haus nicht oder Atemnot beim Ankleiden

### BMI

`imc`

kg/m² · Bereich: 10–70

## Fassung der Methode

BODE/Celli 2004: BMI/FEV₁/mMRC/6MWD, gesamt 0–10; Original, kein aktualisierter BODE

## Dokumentierte Formel

O (FEV₁ % Soll): ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E (6-Minuten-Gehtest): ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B (BMI): \> 21 = 0; ≤ 21 = 1.

## Grenzen und Population

Der ursprüngliche BODE wurde zur Prognose bei COPD unter Verwendung respiratorischer und systemischer Messungen einschließlich Sechs-Minuten-Gehtest entwickelt. Er diagnostiziert keine COPD und liefert nicht automatisch eine individuelle zeitbezogene Wahrscheinlichkeit; Testbedingungen, Itemdefinitionen und Eignung müssen zur Version passen.

## Referenzen

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
