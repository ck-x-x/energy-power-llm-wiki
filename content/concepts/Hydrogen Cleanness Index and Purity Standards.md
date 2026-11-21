---
type: concept
tags:
  - concept
  - hydrogen-production
  - hydrogen-purity
  - cleanness-index
  - standards
aliases:
  - "氫能潔淨度指數與純度標準"
  - "HCI 與 ISO 14687"
sources_count: 2
updated: 2026-11-21
---

# Hydrogen Cleanness Index and Purity Standards

在氫能系統規劃中，產氫路徑的選擇不能只看轉換效率，還必須同時評估**終端應用純度標準（Purity Standards）**、**純化回收率損耗**以及**全生命週期碳排強度（HCI）** [[Hydrogen Production for Energy Overview (2020)]] [[Hydrogen Energy Economy and Storage Review (2019)]]。

---

## 1. 氫能方形模型（Hydrogen Square, HydS）

Dawood et al. (2020) 提出將氫能系統視為四個互依角點，並強制納入兩大跨角子系統：
- **四角**：生產（Production）↔ 儲存（Storage）↔ 安全（Safety）↔ 應用（Utilisation）。
- **橫跨子系統**：<strong>純化（Purification）</strong>與**壓縮（Compression）**——兩者的 Capex、Opex、能耗與回收率折損常被傳統 TEA 遺漏，卻直接決定化石／生質產氫接入燃料電池時的真實經濟性。

---

## 2. 關鍵純度標準與雜質上限（ISO 14687-2 / SAE J2719）

車用質子交換膜燃料電池（PEMFC，ISO 14687-2 Grade D / SAE J2719）要求乾燥基準純度 **`≥ 99.97%`**，對催化劑毒物設下極嚴格上限 [[Hydrogen Production for Energy Overview (2020)]]：

| 雜質種類 | PEMFC 容許上限 | 工程意義 |
| --- | --- | --- |
| **總硫（含 $\text{H}_2\text{S}$）** | `0.004 ppm` | 極強毒化 Pt 催化劑 |
| **甲醛（$\text{CH}_2\text{O}$） / 氨（$\text{NH}_3$）** | `0.01 ppm` / `0.1 ppm` | 損傷質子交換膜與催化層 |
| **一氧化碳（$\text{CO}$） / 甲酸** | `0.2 ppm` / `0.2 ppm` | 強烈毒化 PEMFC 陽極 Pt 觸媒 |
| **$\text{CO}_2$ / 總碳氫化合物** | `2 ppm` / `2 ppm` | 生質產氫與重組氣須深度脫碳 |
| **$\text{H}_2\text{O}$ / $\text{O}_2$** | `5 ppm` / `5 ppm` | 影響水管理與安全 |
| **$\text{N}_2 + \text{Ar}$ / $\text{He}$** | `100 ppm` / `300 ppm` | 惰性稀釋氣體上限 |

- **純化路徑的純度 vs. 回收率權衡**：
  - **變壓吸附（PSA）**：純度 `98–99.999%`，但回收率僅 **`46–85%`**。
  - **鈀膜（Pd Membrane）**：純度可達 `99.9999%–99.99999%`、回收率 `99%`（[[Hydrogen Energy Economy and Storage Review (2019)]] 與 [[Hydrogen Production for Energy Overview (2020)]] 皆肯定其超高純度，但成本與工作溫度高）。
  - **水電解天然優勢**：[[Water Electrolysis Technologies (AEL, PEM, SOEC)|水電解產氫]] 原生不含 $\text{CO}_x$ 與 $\text{SO}_x$，大幅減輕下游純化負擔。

---

## 3. 氫能潔淨度指數（Hydrogen Cleanness Index, HCI）

- **傳統色彩標籤（灰／藍／綠氫）的缺陷**：僅反映「能源來源或是否加裝 CCS」，無法量化真實碳排（例如生質能產氫雖屬再生，仍可能排放 $\text{CO}_x, \text{SO}_x, \text{CH}_4$；藍氫常漏計上游開採逸散與 CCS 能耗）。
- **HCI 雙維度框架**：以連續百分比色彩光譜（如 `75 Green-2`，對照文獻綠氫上限 `4.4 kg CO2-e / kg H2`）搭配 **4 層評估深度**：
  - **Level 1 (Scope 1)**：產氫過程直接 $\text{CO}_2\text{-e}$ 排放；
  - **Level 2 (Scope 2)**：外購電力／熱能間接排放；
  - **Level 3 (Scope 3)**：第三方全生命週期（LCA）上下游排放；
  - **Level 4 (Scope 4)**：純化子系統所衍生的額外 $\text{CO}_2\text{-e}$ 排放。

---

## 4. 相關知識庫連結
- 來源文獻：[[Hydrogen Production for Energy Overview (2020)]]、[[Hydrogen Energy Economy and Storage Review (2019)]]
- 相關方法：[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Hydrogen Storage Technologies and Metal Hydrides]]
- 全五篇綜合比較：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]
