---
type: method
category: "storage"
tags:
  - method
  - hydrogen-storage
  - metal-hydrides
  - salt-caverns
aliases:
  - "儲氫技術與金屬氫化物"
  - "固態儲氫改質策略"
sources_count: 3
updated: 2026-11-21
---

# Hydrogen Storage Technologies and Metal Hydrides

氫氣質量熱值極高（LHV `120 MJ/kg = 33.33 kWh/kg`），但常壓體積密度極低（`0.089 kg/m³`，LHV `11 MJ/m³`），如何兼顧安全、體積、能耗與成本是氫能商業化的最大瓶頸 [[Hydrogen Energy Economy and Storage Review (2019)]] [[Hydrogen Production for Energy Overview (2020)]] [[Renewable Power-to-Gas Review (2016)]]。

---

## 1. 物理儲氫 vs. 固態儲氫對比
> **壓力單位 SI 換算註記**：`1 bar = 0.1 MPa`、`1 atm = 101.325 kPa`（下表保留各論文原始壓力單位）。

| 儲氫路線 | 操作條件 | 能量損耗／容量特徵 | 適用場景與核心瓶頸 |
| --- | --- | --- | --- |
| **高壓氣態儲氫** | `35–70 MPa`（PtG 緩衝 `350–700 bar`） | 壓縮能耗佔氫能 **`11–13%`** | 目前車載與 PtG 現場緩衝主力；碳纖複合瓶（CFRP）昂貴且有高壓安全疑慮 |
| **地下鹽穴儲氫** | 高壓地質鹽丘洞穴（具體壓深原文未提供） | 極低滲透、單位成本最低 | 季節性大規模儲能（如歐盟 **HyUnder** 羅馬尼亞計畫）；受地質場址限制 |
| **低溫液態儲氫（$\text{LH}_2$）** | `20 K`（`-252.8 °C`），密度 `~71 kg/m³`（`8 MJ/L`） | 液化能耗高達 **`~30%`** + 持續蒸發（boil-off） | 航太與短期高能量密度需求；絕熱槽昂貴、不適合長期靜置 |
| **固態物理吸附** | 碳奈米管、MOF、沸石、活性碳 | 動力學快、完全可逆 | 常溫儲量過低，仍需低溫操作 |
| **固態化學氫化物** | 如 $\text{NaBH}_4$ 水解 | 理論達 `10.8 wt.%` | 反應放熱過大、**不可逆**（需車外再生） |
| **可逆金屬氫化物** | 溫和壓力 **`3–30 atm`**（`0.30–3.04 MPa`） | 高體積原子堆積密度、兼具儲熱功能 | 低溫合金太重（`< 2 wt.%`）；高溫 $\text{MgH}_2$ 儲量高（`7.6 wt.%`）但需 `300–400 °C` |

> [!warning] 觀點衝突 / 條件差異：液態氫密度數值微小差異（Abe 2019 vs. Dawood 2020）
> - **[[Hydrogen Energy Economy and Storage Review (2019)]]**：引用 `20 K` 下液態氫密度約 **`71 kg/m³`**（氣態 LHV `119.96 MJ/kg`）。
> - **[[Hydrogen Production for Energy Overview (2020)]]**：Table 2 記載正常沸點（`-252.8 °C`, `101.283 kPa`）下液態氫密度為 **`67.76 kg/m³`**（氣態 LHV `120 MJ/kg`）。約 `4.5%` 之密度差異源於參考溫度與飽和／過冷液態基準點不同。

---

## 2. 代表性金屬氫化物與四大改質策略（Abe et al., 2019）

可逆反應：$\text{M} + \frac{x}{2}\text{H}_2 \rightleftharpoons \text{MH}_x + Q$

| 類別 | 代表材料 | 儲氫量（`wt.%`） | 平衡壓力（`bar`） | 操作溫度（`K`） |
| --- | --- | --- | --- | --- |
| $\text{AB}_5$ | $\text{LaNi}_5\text{H}_6$ | `1.4` | `2` | `298` |
| $\text{AB}$ | $\text{FeTiH}_2$ | `1.89` | `5` | `303` |
| BCC 固溶體 | $\text{TiV}_2\text{H}_4$ | `2.60` | `10` | `313` |
| $\text{AB}_2$ | $\text{ZrV}_2\text{H}_{5.5}$ | `3.01` | $10^{-8}$ | `323` |
| $\text{A}_2\text{B}$ | $\text{Mg}_2\text{NiH}_4$ | `3.59` | `1` | `555` |
| 單質輕金屬 | $\text{MgH}_2$ | **`7.6`** | `1` | `600` |

### 針對 $\text{MgH}_2$ 的四大改質工程
1. **催化（Catalysis）**：$\text{Nb}_2\text{O}_5$ 表現最佳（`300 °C` 下 `60 s` 吸氫 `7 wt.%`、`130 s` 放氫；`1 mol%` 使吸氫 $E_a$ 降至 `38 kJ/mol`），但**不改變熱力學穩定度**。
2. **合金化（Alloying）**：加 `5%` V 球磨使放氫 $E_a$ 由 `120` 降至 `62.3 kJ/mol`；$\text{Mg}_2\text{Ni}$ 與 $\text{Cu}_2\text{Mg}$ 可將 `1 bar` 平衡放氫溫降至 `240–245 °C`（熱力學去穩定化）。
3. **奈米結構化（Ball Milling）**：破壞表面氧化鈍化層（SPL）、縮短擴散路徑；量子計算指出 `~0.9 nm` 團簇可於 `200 °C` 放氫。
4. **奈米限域（Nanoconfinement）**：將 `~3 nm` $\text{MgH}_2$ 嵌入微孔碳／碳氣凝膠骨架防止燒結，放氫 $E_a$ 降 `52 kJ/mol`、放氫溫由 `400 °C` 降至 `200 °C`、放氫速率提升 `> 5×`（權衡：孔徑越小動力學越快，但有效裝載量下降）。

---

## 3. 相關知識庫連結
- 來源文獻：[[Hydrogen Energy Economy and Storage Review (2019)]]、[[Hydrogen Production for Energy Overview (2020)]]、[[Renewable Power-to-Gas Review (2016)]]
- 上下游連結：[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Power-to-Gas and Methanation Processes]]
- 全五篇綜合比較：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]
