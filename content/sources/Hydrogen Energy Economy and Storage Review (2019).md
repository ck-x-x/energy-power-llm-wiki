---
type: source
title: "Hydrogen energy, economy and storage: Review and recommendation"
authors:
  - "J.O. Abe"
  - "A.P.I. Popoola"
  - "E. Ajenifuja"
  - "O.M. Popoola"
year: 2019
venue: "International Journal of Hydrogen Energy, Vol. 44, pp. 15072–15086"
doi: "10.1016/j.ijhydene.2019.04.068"
raw_file: "raw/papers/Hydrogen energy economy and storage Review.pdf"
status: ingested
tags:
  - source
  - hydrogen-economy
  - hydrogen-storage
  - metal-hydrides
  - energy-carrier
aliases:
  - "Abe et al. (2019) Hydrogen Storage Review"
  - "氫能經濟與儲氫技術綜述 (2019)"
updated: 2026-11-21
---

# Hydrogen Energy Economy and Storage Review (2019)

> **原始論文**：`raw/papers/Hydrogen energy economy and storage Review.pdf`  
> **出處**：J.O. Abe, A.P.I. Popoola, E. Ajenifuja, O.M. Popoola, *International Journal of Hydrogen Energy* 44 (2019) 15072–15086

---

## 1. 核心貢獻（TL;DR）

1. **儲氫是氫能經濟的核心瓶頸**：指出氫氣具備極高質量能量密度（LHV `119.96 MJ/kg = 33.33 kWh/kg`，HHV `141.88 MJ/kg`，逾常規汽油 `43.44 MJ/kg` 的 `2.7` 倍），但常溫常壓密度僅 `0.089 kg/m³`，因此安全、緊湊、低成本的儲氫技術是邁向氫能經濟的最大門檻。
2. **全面評估三大儲氫路線**：比較高壓氣態（`35–70 MPa` 與地下鹽穴）、低溫液態（`20 K`）與固態儲氫（物理吸附 vs. 化學吸附），認為傳統壓縮（損耗 `11–13%`）與液化（損耗 `~30%` 且持續蒸發 boil-off）難以同時滿足車載安全、體積與成本目標。
3. **鎖定可逆金屬氫化物（Metal Hydrides）**：在溫和壓力（`3–30 atm`）下提供高體積原子堆積密度與高安全性，剖析低溫金屬間化合物（`< 2 wt.%`、重且貴）與高溫輕質氫化物（如 $\text{MgH}_2$ 達 `7.6 wt.%`、但需 `300–400 °C` 且動力學緩慢）的兩難。
4. **推薦四大材料改質工程路徑**：系統評述**催化（Catalysis）**、**合金化（Alloying）**、**奈米結構化（Nanostructuring）**與**奈米限域（Nanoconfinement）**對 $\text{MgH}_2$ 等金屬氫化物之吸放氫動力學與熱力學改質成效，對照 **U.S. DOE 車載儲氫技術目標**。

---

## 2. 研究背景與工程痛點

- 化石燃料佔全球能源供應逾 `80%`（論文引用儲量估算上限：石油 `40 yr`、天然氣 `60 yr`、煤炭 `156 yr`）；歐盟規劃 2050 年建成氫能經濟、2040 年 `35%` 新車採用零碳氫能。
- 傳統物理儲氫痛點：高壓氣瓶需昂貴碳纖維複合材料（CFRP）且具洩漏／碰撞疑慮；液氫需雙層絕熱低溫槽與極高液化能耗；固態化學氫化物（如 $\text{NaBH}_4$ 水解理論 `10.8 wt.%`）不可逆且反應熱過大，不利車載再生。

---

## 3. 系統模型、拓撲與控制方法

### 可逆金屬氫化物吸放氫反應式
$$\text{M} + \frac{x}{2}\text{H}_2 \rightleftharpoons \text{MH}_x + Q$$

- 吸氫過程依序經歷：表面物理吸附 → $\text{H}_2$ 解離為氫原子 → 擴散進入金屬間隙形成固溶體（$\alpha$-phase）→ 氫化物（$\beta$-phase）成核成長至飽和。

### 符號與 SI 單位對照表

| 符號 | 物理意義 | 單位 | 代表數值與條件 |
| --- | --- | --- | --- |
| $\text{M}, \text{MH}_x$ | 金屬／合金及其氫化物 | — | 如 $\text{LaNi}_5\text{H}_6$ (`1.4 wt.%`), $\text{MgH}_2$ (`7.6 wt.%`) |
| $Q$ / $\Delta H$ | 反應熱／生成焓 | `kJ/mol` | $\text{MgH}_2$: `-75 kJ/mol`；$\text{Mg}_2\text{NiH}_4$: `-64.5 kJ/mol`；奈米限域 $\text{MgH}_2$: `63.8 ± 0.5 kJ/mol` |
| $E_a$ | 吸／放氫活化能 | `kJ/mol` | 純 $\text{MgH}_2$ `120` → 加 5% V 降至 `62.3` → 加 `1 mol% Nb2O5` 吸氫降至 `38` |
| $w_{\text{H}_2}$ | 重量儲氫密度 | `wt.%` | DOE 系統目標：`4.5` (2020) → `5.5` (2025) → `6.5 wt.%` (Ultimate) |

---

## 4. 測試系統、工況條件與關鍵實驗／模擬數據

### 4.1 U.S. DOE 輕型燃料電池車（FCV）車載儲氫目標（Table 2）

| 指標 | 單位 | 2020 | 2025 | Ultimate |
| --- | --- | --- | --- | --- |
| 系統重量儲氫容量 | `kg H2 / kg system`（`kWh/kg` 材料） | `0.045` (`1.5`) | `0.055` (`1.8`) | `0.065` (`2.2`) |
| 系統體積儲氫容量 | `kg H2 / L system`（`kWh/L` 材料） | `0.030` (`1.0`) | `0.040` (`1.3`) | `0.050` (`1.7`) |
| 儲氫系統成本 | `$/kWh net`（`$/kg H2`） | `10` (`333`) | `9` (`300`) | `8` (`266`) |
| 循環壽命 / 充氣時間（4–10 kg） | `cycles` / `min` | `1,500` / `3–5 min` | `1,500` / `3–5 min` | `1,500` / `3–5 min` |
| 供氣壓力 / 純度標準 | `bar` / `%` | `5–12 bar` / SAE J2719 (`99.97%`) | 同左 | 同左 |

### 4.2 四大材料改質關鍵數據與地質儲氫實例
> **單位換算註記**：本頁壓力保留原文單位，對應 SI 換算為 `1 bar = 0.1 MPa`、`1 atm = 101.325 kPa`。

- **催化（$\text{MgH}_2 + \text{Nb}_2\text{O}_5$）**：於 `300 °C` 下 `60 s` 吸氫 `7 wt.%`、`130 s` 放氫（最佳氧化物催化順序：$\text{Nb}_2\text{O}_5 > \text{Fe}_3\text{O}_4 > \text{CeO}_2 > \text{ZrO}_2$）；另一研究降至 `205 °C` 放氫；添加 `1 mol% Nb2O5` 可於 `-50 °C` 吸氫（$E_a = 38\ \text{kJ/mol}$，具體吸氫壓力原文未提供）。
- **合金化**：$\text{MgH}_2 + 5\%$ V 球磨 `20 h` 使放氫 $E_a$ 由 `120` 降至 `62.3 kJ/mol`（具體測試溫壓原文未提供）；$\text{Mg}_2\text{Ni}$ 在 `1 bar` (`0.1 MPa`) 下平衡放氫溫度降至 `245 °C`（`3.6 wt.%`）。
- **奈米限域**：`~3 nm` $\text{MgH}_2$ 嵌入微孔碳骨架使放氫 $E_a$ 降低 `52 kJ/mol`、放氫溫度由 `400 °C` 降至 `200 °C`（具體背壓原文未提供）；`~13 nm` 碳氣凝膠載體使放氫動力學較球磨樣品快逾 `5` 倍（具體背壓原文未提供）。
- **地下鹽穴儲氫**：歐盟 FCH JU 資助之 **HyUnder** 計畫（羅馬尼亞案例）利用極低滲透率鹽丘洞穴進行季節性大規模儲氫，於無風無光期供應複循環電廠發電（具體操作壓力與洞穴深度原文未提供）。

---

## 5. 假設條件、工程限制與未解問題

1. **表面鈍化層（SPL）與毒化**：活潑金屬（Mg, FeTi）表面易氧化成阻氣層，需高溫高壓真空活化，且易不可逆氧化造成有效儲量衰減。
2. **貴金屬催化與孔洞載體成本**：Pd、Pt、Ru 等催化劑過於昂貴；MOF、沸石與介孔氧化物支架因自重與成本限制實際系統重量密度。
3. **奈米限域的裝載量權衡**：較小孔徑雖加快放氫動力學，但同時降低 $\text{MgH}_2$ 有效填充比例。

---

## 6. 知識庫關聯與觀點衝突

- **核心方法**：[[Hydrogen Storage Technologies and Metal Hydrides]]
- **上下游連結**：[[Hydrogen Production for Energy Overview (2020)]]、[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Power-to-Gas and Methanation Processes]]
- **全五篇綜合比較**：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]

> [!warning] 觀點衝突 / 條件差異：催化劑能加速動力學，但無法打破熱力學穩定度上限
> - **動力學突破**：加入 `1 mol% Nb2O5` 催化劑可將 $\text{MgH}_2$ 吸氫活化能 $E_a$ 大幅壓低至 `38 kJ/mol`（甚至於 `-50 °C` 吸氫），但**並未改變 $\text{MgH}_2$ 本身的熱力學放氫焓與平衡溫度**。
> - **熱力學去穩定化**：必須結合**合金化**（如 $\text{Mg}_2\text{Ni}$ 降至 `-64.5 kJ/mol`）或**奈米限域**（`~3 nm` 碳孔隙降至 `63.8 kJ/mol`、`200 °C` 放氫），方能同時降低操作溫度。
