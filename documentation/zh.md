<!-- ELUCENIA technical documentation · relacao-pao2-fio2 · zh · no clinical/professional/rights approval -->

# PaO₂/FiO₂ 比值与 ARDS（Berlin 定义）

[条件、来源与许可](https://elucenia.org/zh/tools/relacao-pao2-fio2)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### PaO₂

`pao2`

mmHg · 范围: 20–700

### FiO₂

`fio2`

% · 范围: 21–100

### PEEP 或 CPAP

`peep`

cmH₂O · 选填 · 范围: 0–30

### SpO₂（用于 SpO₂/FiO₂ 比值）

`spo2`

% · 选填 · 范围: 50–100

## 方法版本

柏林ARDS 2012：P/F 100/200/300+PEEP/背景；2024全球定义S/F成分，SpO₂≤97

## 已记录的公式

P/F比 = PaO₂ (mmHg) ÷ FiO₂ (小数: 40% = 0.40).

SpO₂/FiO₂ = SpO₂ (%) ÷ FiO₂ (小数), 可解释条件 SpO₂ ≤ 97%.

## 限制与适用人群

P/F比仅是急性呼吸窘迫综合征（ARDS）定义的一部分。Berlin分类除了氧合阈值，还需要最终定义中的其他条件；单独比值不能确诊ARDS。S/F分类属于后续全球定义，需采用其自身标准，不能混入从Berlin草案中删除的辅助变量。

## 参考文献

- [ARDS Definition Task Force; Ranieri VM et al. Acute respiratory distress syndrome: the Berlin Definition. JAMA, 2012.](https://doi.org/10.1001/jama.2012.5669)

- [Matthay MA et al. A new global definition of acute respiratory distress syndrome. Am J Respir Crit Care Med, 2024.](https://doi.org/10.1164/rccm.202303-0558WS)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
