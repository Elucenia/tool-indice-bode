<!-- ELUCENIA technical documentation · indice-bode · pt-BR · no clinical/professional/rights approval -->

# Índice BODE

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/indice-bode)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### VEF₁ pós-broncodilatador

`vef1`

% do previsto · intervalo: 5–150

### Distância no teste de caminhada de 6 minutos

`dist`

m · intervalo: 0–1000

### Dispneia (escala mMRC)

`mmrc`

- `0` — 0: só com exercício intenso
- `1` — 1: ao andar rápido ou subir ladeira
- `2` — 2: anda mais devagar que pessoas da mesma idade ou para ao andar no plano
- `3` — 3: para após ~100 m ou poucos minutos no plano
- `4` — 4: não sai de casa ou tem dispneia ao se vestir

### IMC

`imc`

kg/m² · intervalo: 10–70

## Edição do método

BODE/Celli 2004:IMC/VEF 1/m MRC/6 MWD, total 0–10; original, semupdated BODE

## Fórmula documentada

O (VEF₁ % previsto): ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E (caminhada de 6 min): ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B (IMC): \> 21 = 0; ≤ 21 = 1.

## Limites e população

O BODE original foi desenvolvido para prognóstico em DPOC utilizando medidas respiratórias e sistêmicas, inclusive caminhada de seis minutos. Não diagnostica DPOC nem fornece automaticamente probabilidade individual por prazo; condições de teste, definições dos itens e elegibilidade devem corresponder à versão.

## Referências

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
