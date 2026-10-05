<!-- ELUCENIA technical documentation · indice-bode · es · no clinical/professional/rights approval -->

# Índice BODE

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/indice-bode)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### VEF₁ posbroncodilatador

`vef1`

% del valor previsto · intervalo: 5–150

### Distancia en la prueba de marcha de 6 minutos

`dist`

m · intervalo: 0–1000

### Disnea (escala mMRC)

`mmrc`

- `0` — 0: solo con ejercicio intenso
- `1` — 1: al caminar deprisa o subir una cuesta
- `2` — 2: camina más despacio que personas de la misma edad o se detiene al caminar en llano
- `3` — 3: se detiene tras ~100 m o pocos minutos en llano
- `4` — 4: no sale de casa o tiene disnea al vestirse

### IMC

`imc`

kg/m² · intervalo: 10–70

## Edición del método

BODE/Celli 2004: IMC/VEF₁/mMRC/6MWD, total 0–10; original, sin BODE actualizado

## Fórmula documentada

O (VEF₁ % predicho): ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E (marcha de 6 min): ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B (IMC): \> 21 = 0; ≤ 21 = 1.

## Límites y población

El BODE original se desarrolló para el pronóstico en EPOC utilizando medidas respiratorias y sistémicas, incluida la caminata de seis minutos. No diagnostica EPOC ni proporciona automáticamente una probabilidad individual para un plazo; las condiciones de la prueba, las definiciones de los ítems y la elegibilidad deben corresponder a la versión.

## Referencias

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
