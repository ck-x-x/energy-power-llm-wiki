---
type: source
title: "Hydrogen production for energy: An overview"
authors:
  - "Furat Dawood"
  - "Martin Anda"
  - "G.M. Shafiullah"
year: 2020
venue: "International Journal of Hydrogen Energy, Vol. 45, pp. 3847–3869"
doi: "10.1016/j.ijhydene.2019.12.059"
raw_file: "raw/papers/Hydrogen production for energy An overview.pdf"
status: ingested
tags:
  - source
  - hydrogen-production
  - hydrogen-purity
  - cleanness-index
  - lca
aliases:
  - "Dawood et al. (2020) Hydrogen Production Overview"
  - "能源用氫氣生產途徑與潔淨度綜述 (2020)"
updated: 2026-11-21
---

# Hydrogen Production for Energy Overview (2020)

> **原始論文**：`raw/papers/Hydrogen production for energy An overview.pdf`  
> **出處**：F. Dawood, M. Anda, G.M. Shafiullah, *International Journal of Hydrogen Energy* 45 (2020) 3847–3869

---

## 1. 核心貢獻（TL;DR）

1. **氫能方形生命週期模型（Hydrogen Square, HydS）**：提出涵蓋**生產（Production）、儲存（Storage）、安全（Safety）、應用（Utilisation）**四角的整合系統模型，並將**純化（Purification）與壓縮（Compression）**列為橫跨各角的關鍵子系統，補齊過往 300 餘篇文獻各自為政的缺口。
2. **三層級產氫途徑分類與成熟度（TML 1–10）**：依「輸入能源型態 → 含氫原料（烴類 H / 非烴類 N）→ 技術／催化劑」系統評估 11 大類產氫路徑的轉換效率、潔淨度（C / N / CCS）與整合技術成熟度（TML 1–10，融合 NASA TRL 1–9 與 ARENA CRI 1–6）。
3. **將純度標準與純化成本納入技術經濟評估**：強調燃料電池（PEMFC）要求嚴苛純度（ISO 14687-2 Grade D / SAE J2719：`> 99.97%`、$\text{CO} \le 0.2\ \text{ppm}$、總硫 $\le 0.004\ \text{ppm}$），而不同純化技術（如 PSA 回收率僅 `46–85%` vs. 鈀膜 `99%`）直接左右產氫路徑的真實成本與回收率。
4. **提出氫能潔淨度指數（Hydrogen Cleanness Index, HCI）**：批判傳統「灰氫／藍氫／綠氫」離散色彩標籤僅代表能源來源而非真實全生命週期碳排，提出連續光譜百分比搭配 **4 層評估深度（Scope 1 直接碳排 → Scope 4 純化碳排）** 的量化框架（例如 `75 Green-2`）。

---

## 2. 研究背景與工程痛點

- 2016 年全球工業產氫量達 **`8,500 萬噸`（逾 `6,000 億 Nm³/yr`）**，其中約 `95–96%` 來自化石燃料重組／裂解，**再生能源水電解佔比僅 `4–5%`**。
- 氫氣體積能量密度極低（常壓 LHV 僅 `11 MJ/m³`、液氫 `8 MJ/L`，僅為汽油 `32 MJ/L` 的 `1/4`），加上寬可燃範圍（空氣中 `4%–75%`）、極低點火能（汽油的 `1/10`）與金屬氫脆風險，且分析顯示逾 `70%` 氫能事故源於組織與人為因素，使安全與純度成為商業化硬約束。

---

## 3. 系統模型、拓撲與控制方法

*(註：本論文為系統層級分類與生命週期整合綜述，原文未提供個別化學反應方程式、反應焓或反應器溫壓數據，核心貢獻為效率定義、熱物性基準、HydS 與 HCI 框架。)*

- **產氫效率通式**：$\eta_{\text{HPP}} = \dfrac{\text{產出 }\text{H}_2\text{ 能量值}}{\text{生產過程總投入能量}}$（氨分解因工業氨先由氫氣合成，故歸為儲運介質而非一次產氫途徑）。

### 符號與 SI 單位對照表（Table 2 熱物性基準）

| 符號／指標 | 物理意義 | SI 單位（或原文單位） | 原文記載數值與工況條件 |
| --- | --- | --- | --- |
| $\eta_{\text{HPP}}$ | 產氫途徑總轉換效率 | `%`（無因次） | 依路徑 `0.5%–90%`（詳見第 4 節） |
| $\text{LHV}_m, \text{HHV}_m$ | 質量低／高熱值 | $\text{MJ/kg}$ | `120` / `141.8`（`298 K`） |
| $\text{LHV}_v, \text{HHV}_v$ | 體積低／高熱值 | $\text{MJ/m}^3$ | `11` / `13`（`1 atm = 101.325 kPa`）；液氫 `8 MJ/L` |
| $T_b, T_m$ | 沸點／熔點 | $^\circ\text{C}$（$\text{K}$） | `-252.8 °C` (`20.35 K`) / `-259.2 °C` (`13.95 K`) @ `101.283 kPa` |
| $h_{fg}$ | 氣化潛熱 | $\text{kJ/kg}$ | `445.6`（沸點條件） |
| $T_c, P_c, \rho_c$ | 臨界溫度／壓力／密度 | $^\circ\text{C}$, $\text{kPa}$, $\text{kg/m}^3$ | `-239.9 °C` / `1,296.212 kPa (abs)` / `30.12 kg/m³` |
| $\rho_l, \rho_g$ | 液相／沸點氣相密度 | $\text{kg/m}^3$ | `67.76`（液相） / `1.331`（沸點、`1 atm` 氣相） |
| $D_{\text{H}_2\text{–air}}$ | 空氣中分子擴散係數 | $\text{m}^2/\text{s}$ | $6.1 \times 10^{-5}$ |
| 可燃／爆炸界限 | 空氣中體積濃度範圍 | `vol.%` | 可燃 `4%–75%`；爆炸 `18.2–58.9 vol.%` |
| 雜質上限 | PEMFC 容許濃度（ISO 14687-2） | `ppm`（莫耳／體積分率 $\mu\text{mol/mol}$） | $\text{CO} \le 0.2\ \text{ppm}$、總硫 $\le 0.004\ \text{ppm}$ |

---

## 4. 測試系統、工況條件與關鍵實驗／模擬數據

### 4.1 主要產氫途徑效率、潔淨度與成熟度對比（Table 4 & Table 5）

| 產氫技術 | 能源輸入 | 原料 | 效率（%） | 潔淨度 | TML（1–10） |
| --- | --- | --- | --- | --- | --- |
| **鹼性電解（AE）** | 電能 | 水（N） | `62–82` | C | `9–10` |
| **質子交換膜電解（PEM）** | 電能 | 水（N） | `67–84` | C | `7–9` |
| **固態氧化物電解（SOC）** | 電能（+熱） | 水（N） | `75–90` | C | `3–5` |
| **蒸汽重組（SR / SMR）** | 熱能 | 化石燃料（H） | `60–85` | N / CCS | `10` |
| **煤炭氣化** | 熱能 | 煤（H） | `74–85` | N / CCS | `10` |
| **膜反應器（Membrane Reactor）** | 熱能 | 燃料（H） | `64–90` | N / CCS | `7–9` |
| **生質氣化／熱解** | 熱能 | 生質能（H） | `35–50` | N | `8–10` |
| **微生物電解 / 暗發酵** | 生質（+電） | 生質（H） | `70–80` / `60–80` | N | `1–3` / `3–5` |
| **光電化學（PEC） / 光催化** | 光（+電） | 水（N） | `0.5–12` / `3–11` | C | `1–2` |
| **新興：Battolyser（電池+電解一體）** | 電能 | 水（N） | `76–90`（整體） | C | 新興研發 |
| **新興：一體化再生燃料電池（URFC）** | 電能 | 水（N） | `43–51`（往返） | C | 新興研發 |

### 4.2 氫氣純化技術對比（Table 9）與碳排門檻
- **鈀膜（Pd Membrane）**：純度 `99.99999%`、回收率 `99%`（瓶頸：降本與降工作溫度）。
- **變壓吸附（PSA）**：純度 `98–99.999%`、回收率僅 **`46–85%`**（純度與回收率強烈權衡）。
- **低溫分離（Cryogenic）**：純度 `95–99.8%`、回收率 `95%`；**金屬氫化物純化**：純度 `99–99.99%`、回收率 `75–95%`。
- **綠氫碳排門檻引用值**：文獻認定之綠氫碳排上限為 **`4.4 kg CO2-e / kg H2`**。*(註：原論文未提供各路徑具體 `$/kg H2` 生產成本數據，原文未提供。)*

---

## 5. 假設條件、工程限制與未解問題

1. **「全面氫能經濟」的可行性存疑**：多數綜述文獻認為短期內無法建成完全依賴氫能的經濟體，氫能應定位為低碳智慧能源系統中的**互補載體**（HydESS 跨小時至季節儲能、重工業與長途運輸）。
2. **HCI 模型仍屬概念框架**：需後續研究訂定各色帶邊界門檻與 Scope 1–4 的權重計算規則。
3. **純化與壓縮常被忽略**：過往技術經濟分析（TEA）遺漏純化 Capex/Opex 與回收率折損，低估了化石／生質產氫接入 PEMFC 時的真實成本。

---

## 6. 知識庫關聯與觀點衝突

- **核心概念**：[[Hydrogen Cleanness Index and Purity Standards]]
- **核心方法**：[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Hydrogen Storage Technologies and Metal Hydrides]]、[[Power-to-Gas and Methanation Processes]]
- **全五篇綜合比較**：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]

> [!warning] 觀點衝突 / 條件差異：「綠氫」一定比「藍氫」更乾淨嗎？
> - **傳統色彩分類盲點**：以能源來源劃分灰／藍／綠氫時，忽略了部分再生路徑（如生質能產氫會排放 $\text{CO}_x$、$\text{SO}_x$、$\text{CH}_4$，或再生熱源排放 $\text{N}_2\text{O}$/$\text{NO}_x$）仍具溫室氣體排放；同時藍氫常遺漏上游化石開採逸散與 CCS 能耗。
> - **論文主張（HCI 模型）**：應以全生命週期 $\text{CO}_2\text{-e}$ 量化光譜（納入 Scope 1–4 含純化碳排）取代粗糙的顏色標籤。
