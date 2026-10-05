<!-- ELUCENIA technical documentation · indice-bode · zh · no clinical/professional/rights approval -->

# BODE 指数

[条件、来源与许可](https://elucenia.org/zh/tools/indice-bode)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 支气管舒张后 FEV₁

`vef1`

%预计值 · 范围: 5–150

### 6 分钟步行试验距离

`dist`

m · 范围: 0–1000

### 呼吸困难（mMRC 量表）

`mmrc`

- `0` — 0：仅在剧烈运动时
- `1` — 1：快走或上坡时
- `2` — 2：比同龄人走得慢，或平地行走时需要停下
- `3` — 3：平地行走~100 m或数分钟后停下
- `4` — 4：不外出或穿衣时呼吸困难

### 体重指数（BMI）

`imc`

kg/m² · 范围: 10–70

## 方法版本

BODE/Celli 2004：BMI/FEV₁/mMRC/6MWD，总分0–10；原版，非更新BODE

## 已记录的公式

O（FEV₁占预计值%）： ≥ 65 = 0; 50–64 = 1; 36–49 = 2; ≤ 35 = 3.
E（6分钟步行）： ≥ 350 m = 0; 250–349 = 1; 150–249 = 2; ≤ 149 = 3.
D (mMRC): 0–1 = 0; 2 = 1; 3 = 2; 4 = 3.
B（BMI）： \> 21 = 0; ≤ 21 = 1.

## 限制与适用人群

原始BODE为慢性阻塞性肺疾病（COPD）预后而开发，采用呼吸及全身性测量，包括六分钟步行。它不能诊断COPD，也不会自动提供特定时间范围的个体概率；测试条件、项目定义及适用资格须与版本一致。

## 参考文献

- [Celli BR et al. The body-mass index, airflow obstruction, dyspnea, and exercise capacity index in chronic obstructive pulmonary disease. N Engl J Med, 2004.](https://doi.org/10.1056/NEJMoa021322)

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
