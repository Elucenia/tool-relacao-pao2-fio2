<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · pt-BR · no clinical/professional/rights approval -->

# Relação PaO₂/FiO₂ e SDRA (Berlim)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/relacao-pao2-fio2)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### PaO₂

`pao2`

mmHg · intervalo: 20–700

### FiO₂

`fio2`

% · intervalo: 21–100

### PEEP ou CPAP

`peep`

cmH₂O · opcional · intervalo: 0–30

### SpO₂ (para a relação SpO₂/FiO₂)

`spo2`

% · opcional · intervalo: 50–100

## Edição do método

Berlin ARDS 2012:PFratio 100/200/300+PEEP/contexto; SFratio componente Global Definition 2024, Sp O 2≤97

## Fórmula documentada

Relação P/F = PaO₂ (mmHg) ÷ FiO₂ (em fração: 40% = 0,40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (fração), interpretável com SpO₂ ≤ 97%.

## Limites e população

A relação P/F é apenas um componente da definição de SDRA. Classificação de Berlim exige as demais condições da definição final, além dos limites de oxigenação; razão isolada não confirma SDRA. A classificação por S/F pertence à definição global posterior e requer critérios próprios, sem misturar variáveis auxiliares retiradas do rascunho de Berlim.

## Referências

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

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
