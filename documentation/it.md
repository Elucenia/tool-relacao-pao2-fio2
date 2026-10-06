<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · it · no clinical/professional/rights approval -->

# Rapporto PaO₂/FiO₂ e ARDS (Berlino)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/relacao-pao2-fio2)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### PaO₂

`pao2`

mmHg · intervallo: 20–700

### FiO₂

`fio2`

% · intervallo: 21–100

### PEEP o CPAP

`peep`

cmH₂O · facoltativo · intervallo: 0–30

### SpO₂ (per il rapporto SpO₂/FiO₂)

`spo2`

% · facoltativo · intervallo: 50–100

## Edizione del metodo

Berlino ARDS 2012: P/F 100/200/300+PEEP/contesto; S/F Definizione Globale 2024, SpO₂≤97

## Formula documentata

Rapporto P/F = PaO₂ (mmHg) ÷ FiO₂ (frazione: 40% = 0,40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (frazione), interpretabile con SpO₂ ≤ 97%.

## Limiti e popolazione

Il rapporto P/F è soltanto una componente della definizione di ARDS. La classificazione di Berlino richiede le altre condizioni della definizione finale, oltre ai limiti di ossigenazione; il solo rapporto non conferma l’ARDS. La classificazione S/F appartiene alla successiva definizione globale e richiede criteri propri, senza mescolare variabili ausiliarie eliminate dalla bozza di Berlino.

## Riferimenti

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

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

Rapporto sopra 300: nessun criterio di ossigenazione per la ARDS


### 2

ARDS lieve secondo il criterio di Berlino (200 a 300)

L’ossigenazione è solo uno dei criteri: esordio entro 1 settimana, opacità bilaterali ed edema non spiegato da insufficienza cardiaca o ipervolemia.


### 3

ARDS moderata secondo il criterio di Berlino (100 a 200)

L’ossigenazione è solo uno dei criteri: esordio entro 1 settimana, opacità bilaterali ed edema non spiegato da insufficienza cardiaca o ipervolemia.


### 4

ARDS grave secondo il criterio di Berlino (≤ 100)

| Dettagli del risultato | |
| --- | --- |
| SpO₂/FiO₂ | 113 (≤ 315: criterio di ipossiemia della definizione globale 2023) |

L’ossigenazione è solo uno dei criteri: esordio entro 1 settimana, opacità bilaterali ed edema non spiegato da insufficienza cardiaca o ipervolemia.

