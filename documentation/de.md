<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · de · no clinical/professional/rights approval -->

# PaO₂/FiO₂-Verhältnis und ARDS (Berlin)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/relacao-pao2-fio2)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### PaO₂

`pao2`

mmHg · Bereich: 20–700

### FiO₂

`fio2`

% · Bereich: 21–100

### PEEP oder CPAP

`peep`

cmH₂O · optional · Bereich: 0–30

### SpO₂ (für das SpO₂/FiO₂-Verhältnis)

`spo2`

% · optional · Bereich: 50–100

## Fassung der Methode

Berlin ARDS 2012: P/F 100/200/300+PEEP/Kontext; S/F globale Definition 2024, SpO₂≤97

## Dokumentierte Formel

P/F-Verhältnis = PaO₂ (mmHg) ÷ FiO₂ (Bruchteil: 40% = 0,40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (Bruchteil), interpretierbar bei SpO₂ ≤ 97%.

## Grenzen und Population

Das P/F-Verhältnis ist nur ein Bestandteil der ARDS-Definition. Die Berlin-Klassifikation erfordert neben Oxygenierungsgrenzen die übrigen Bedingungen der endgültigen Definition; das Verhältnis allein bestätigt kein ARDS. Die S/F-Klassifikation gehört zur späteren globalen Definition und benötigt eigene Kriterien, ohne aus dem Berlin-Entwurf entfernte Hilfsvariablen zu vermischen.

## Referenzen

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Verhältnis über 300: kein Oxygenierungskriterium für ARDS


### 2

Leichtes ARDS nach dem Berlin-Kriterium (200 bis 300)

Die Oxygenierung ist nur eines der Kriterien: Beginn innerhalb von bis zu 1 Woche, bilaterale Opazitäten und ein nicht durch Herzinsuffizienz oder Hypervolämie erklärbares Ödem.


### 3

Mittelgradiges ARDS nach dem Berlin-Kriterium (100 bis 200)

Die Oxygenierung ist nur eines der Kriterien: Beginn innerhalb von bis zu 1 Woche, bilaterale Opazitäten und ein nicht durch Herzinsuffizienz oder Hypervolämie erklärbares Ödem.


### 4

Schweres ARDS nach dem Berlin-Kriterium (≤ 100)

| Ergebnisdetails | |
| --- | --- |
| SpO₂/FiO₂ | 113 (≤ 315: Hypoxämiekriterium der globalen Definition von 2023) |

Die Oxygenierung ist nur eines der Kriterien: Beginn innerhalb von bis zu 1 Woche, bilaterale Opazitäten und ein nicht durch Herzinsuffizienz oder Hypervolämie erklärbares Ödem.

