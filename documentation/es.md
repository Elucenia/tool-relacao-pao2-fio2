<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · es · no clinical/professional/rights approval -->

# Relación PaO₂/FiO₂ y SDRA (Berlín)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/relacao-pao2-fio2)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### PaO₂

`pao2`

mmHg · intervalo: 20–700

### FiO₂

`fio2`

% · intervalo: 21–100

### PEEP o CPAP

`peep`

cmH₂O · opcional · intervalo: 0–30

### SpO₂ (para la relación SpO₂/FiO₂)

`spo2`

% · opcional · intervalo: 50–100

## Edición del método

Berlín SDRA 2012: P/F 100/200/300+PEEP/contexto; S/F de Definición Global 2024, SpO₂≤97

## Fórmula documentada

Relación P/F = PaO₂ (mmHg) ÷ FiO₂ (fracción: 40% = 0,40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (fracción), interpretable con SpO₂ ≤ 97%.

## Límites y población

La relación P/F es solo un componente de la definición de SDRA. La clasificación de Berlín exige las demás condiciones de la definición final, además de los límites de oxigenación; la razón aislada no confirma SDRA. La clasificación por S/F pertenece a la definición global posterior y requiere sus propios criterios, sin mezclar variables auxiliares retiradas del borrador de Berlín.

## Referencias

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

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
