<!-- ELUCENIA technical documentation · indice-bode · it · no clinical/professional/rights approval -->

# Indice BODE

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/indice-bode)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### FEV₁ post-broncodilatatore

`vef1`

% del valore previsto · intervallo: 5–150

### Distanza al test del cammino di 6 minuti

`dist`

m · intervallo: 0–1000

### Dispnea (scala mMRC)

`mmrc`

- `0` — 0: solo con esercizio intenso
- `1` — 1: camminando velocemente o in salita
- `2` — 2: cammina più lentamente dei coetanei o si ferma camminando in piano
- `3` — 3: si ferma dopo ~100 m o pochi minuti in piano
- `4` — 4: non esce di casa o ha dispnea nel vestirsi

### IMC

`imc`

kg/m² · intervallo: 10–70

## Edizione del metodo

BODE/Celli 2004: IMC/FEV₁/mMRC/6MWD, totale 0–10; originale, non BODE aggiornato

## Formula documentata

O (FEV₁ % previsto): ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E (cammino di 6 min): ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B (IMC): \> 21 = 0; ≤ 21 = 1.

## Limiti e popolazione

Il BODE originale è stato sviluppato per la prognosi nella BPCO usando misure respiratorie e sistemiche, incluso il cammino di sei minuti. Non diagnostica la BPCO e non fornisce automaticamente una probabilità individuale per un orizzonte temporale; condizioni del test, definizioni degli item e ammissibilità devono corrispondere alla versione.

## Riferimenti

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
