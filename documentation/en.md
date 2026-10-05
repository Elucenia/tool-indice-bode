<!-- ELUCENIA technical documentation · indice-bode · en · no clinical/professional/rights approval -->

# BODE index

[conditions, sources and permissions](https://elucenia.org/en/tools/indice-bode)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Postbronchodilator FEV₁

`vef1`

% of predicted · range: 5–150

### Six-minute walk test distance

`dist`

m · range: 0–1000

### Dyspnea (mMRC scale)

`mmrc`

- `0` — 0: only with strenuous exercise
- `1` — 1: when hurrying or walking uphill
- `2` — 2: walks slower than people of the same age or stops when walking on level ground
- `3` — 3: stops after ~100 m or a few minutes on level ground
- `4` — 4: housebound or breathless when dressing

### BMI

`imc`

kg/m² · range: 10–70

## Method edition

BODE/Celli 2004: BMI/FEV₁/mMRC/6MWD, total 0–10; original, not updated BODE

## Documented formula

O (FEV₁ % predicted): ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E (6-minute walk): ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B (BMI): \> 21 = 0; ≤ 21 = 1.

## Limits and population

The original BODE was developed for prognosis in COPD using respiratory and systemic measures, including the six-minute walk. It does not diagnose COPD or automatically provide an individual probability for a time horizon; test conditions, item definitions and eligibility must match the version.

## References

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
