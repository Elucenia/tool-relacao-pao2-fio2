<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · en · no clinical/professional/rights approval -->

# PaO₂/FiO₂ ratio and ARDS (Berlin)

[conditions, sources and permissions](https://elucenia.org/en/tools/relacao-pao2-fio2)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### PaO₂

`pao2`

mmHg · range: 20–700

### FiO₂

`fio2`

% · range: 21–100

### PEEP or CPAP

`peep`

cmH₂O · optional · range: 0–30

### SpO₂ (for the SpO₂/FiO₂ ratio)

`spo2`

% · optional · range: 50–100

## Method edition

Berlin ARDS 2012: P/F 100/200/300 plus PEEP/context; S/F component of Global Definition 2024, SpO₂≤97

## Documented formula

P/F ratio = PaO₂ (mmHg) ÷ FiO₂ (fraction: 40% = 0.40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (fraction), interpretable with SpO₂ ≤ 97%.

## Limits and population

The P/F ratio is only one component of the ARDS definition. Berlin classification requires the other conditions of the final definition as well as oxygenation limits; the ratio alone does not confirm ARDS. S/F classification belongs to the later global definition and requires its own criteria, without mixing in auxiliary variables removed from the Berlin draft.

## References

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

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
