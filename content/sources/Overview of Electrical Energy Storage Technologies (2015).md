---
type: source
title: "Overview of current development in electrical energy storage technologies and the application potential in power system operation"
authors:
  - "Xing Luo"
  - "Jihong Wang"
  - "Mark Dooner"
  - "Jonathan Clarke"
year: 2015
venue: "Applied Energy, Vol. 137, pp. 511–536"
doi: "10.1016/j.apenergy.2014.09.081"
raw_file: "raw/papers/Overview of current development in electrical energy storage.pdf"
status: ingested
tags:
  - source
  - electrical-energy-storage
  - power-systems
  - grid-integration
  - commercialization
aliases:
  - "Luo et al. (2015) EES Overview"
  - "電能儲存技術與電力系統應用綜述 (2015)"
updated: 2026-11-21
---

# Overview of Electrical Energy Storage Technologies (2015)

> **原始論文**：`raw/papers/Overview of current development in electrical energy storage.pdf`  
> **出處**：X. Luo, J. Wang, M. Dooner, J. Clarke, *Applied Energy* 137 (2015) 511–536

---

## 1. 核心貢獻（TL;DR）

1. **六大儲能分類全景**：依儲存能量型態將 [[Electrical Energy Storage (EES) Classification|電能儲存（EES）]] 劃分為機械、電化學、電氣、熱化學、化學與熱能六大類（另含複合式 Hybrid EES），系統綜述 266 篇文獻的運作原理、反應式與全球示範專案。
2. **完整定量基準矩陣**：彙整各技術之功率規模（`MW`）、儲能容量（`MWh`）、能量／功率密度（`Wh/L`, `Wh/kg`, `W/L`, `W/kg`）、往返循環效率（`%`）、自放電率、循環與日曆壽命、以及功率／能量單位建置成本（`$/kW`, `$/kWh`）與 O&M 成本。
3. **21 項電力系統應用配對框架**：將電網需求歸納為三大領域（電能品質、橋接／穿越電源、能量管理）共 21 種應用，精準對應功率、響應時間與放電時長至「已實證（Experienced）」與「具潛力（Promising）」技術。
4. **市場現實與季節性儲能缺口**：指出 2012 年全球大型儲能逾 `99%` 仍為抽蓄水力（PHS，`127–129 GW`，約佔全球發電量 `3%`），且截至論文發表時**尚無任何商業化 EES 技術能滿足季節性儲能（30–500 MW、數週至數月）**——此缺口直接銜接 [[Power-to-Gas and Methanation Processes|Power-to-Gas]] 與 [[Hydrogen Storage Technologies and Metal Hydrides|氫能地下儲氣]]。

---

## 2. 研究背景與工程痛點

- 2012 年全球總發電量約 `22,200 TWh`，其中約 `70%` 來自化石燃料；隨風電與光電等間歇性再生能源滲透率提升，電網面臨頻率調節、低電壓穿越（LVRT）、削峰填谷與輸配電升級延緩等迫切挑戰。
- 三大落地障礙：(1) 難以精準匹配 EES 特性與特定電網服務需求；(2) 缺乏實場運轉後的長期技術經濟數據庫；(3) 現行電力市場法規下，除 PHS 外多數技術尚未達成本效益臨界點。

---

## 3. 系統模型、拓撲與控制方法

本論文就機械與電氣儲能之代數能量公式（如 $mgh$、$\frac{1}{2}I\omega^2$、$\frac{1}{2}CV^2$、$\frac{1}{2}LI^2$）**原文未提供**，改以定性物理依賴描述並提供電化學電池與燃料電池核心反應式：

### 核心電化學反應式與單電池電壓
- **鉛酸電池（`2.0 V`）**：$\text{Pb} + \text{SO}_4^{2-} \leftrightarrow \text{PbSO}_4 + 2\text{e}^-$；$\text{PbO}_2 + \text{SO}_4^{2-} + 4\text{H}^+ + 2\text{e}^- \leftrightarrow \text{PbSO}_4 + 2\text{H}_2\text{O}$
- **鋰離子電池（`3.7 V`）**：$\text{C} + n\text{Li}^+ + n\text{e}^- \leftrightarrow \text{Li}_n\text{C}$；$\text{LiXXO}_2 \leftrightarrow \text{Li}_{1-n}\text{XXO}_2 + n\text{Li}^+ + n\text{e}^-$
- **鈉硫電池 NaS（`~2.08 V`, `574–624 K`）**：$2\text{Na} \leftrightarrow 2\text{Na}^+ + 2\text{e}^-$；$x\text{S} + 2\text{e}^- \leftrightarrow x\text{S}^{2-}$
- **全釩液流電池 VRB（`~1.4 V`）**：$\text{V}^{4+} \leftrightarrow \text{V}^{5+} + \text{e}^-$；$\text{V}^{3+} + \text{e}^- \leftrightarrow \text{V}^{2+}$（功率與能量解耦）
- **氫氣燃料電池總反應**：$2\text{H}_2 + \text{O}_2 \rightarrow 2\text{H}_2\text{O} + \text{energy}$（含 AFC、PAFC、SOFC、MCFC、PEMFC、DMFC 六類）

### 關鍵效能指標與 SI 單位對照表

| 指標 | 物理意義 | 單位 | 備註 |
| --- | --- | --- | --- |
| 循環效率（Cycle Efficiency） | 系統總輸出電能 / 總輸入電能 | `%` | 包含充放電轉換與輔助系統損耗 |
| 能量密度 / 比能量 | 單位體積或質量儲能量 | `Wh/L` / `Wh/kg` | 決定佔地面積與移動載具可行性 |
| 功率密度 / 比功率 | 單位體積或質量輸出功率 | `W/L` / `W/kg` | 決定電能品質與瞬態響應能力 |
| 單位功率 / 能量建置成本 | 系統初始投資分攤 | `$/kW` / `$/kWh` | 須搭配 O&M 與循環壽命評估全生命週期成本 |
| 日自放電率（Daily Self-Discharge） | 靜置每日能量損失比例 | `%/day` | 飛輪可達 `100%/day`（`≥20%/h`），PHS/CAES/$\text{H}_2$ 趨近於零 |

---

## 4. 測試系統、工況條件與關鍵實驗／模擬數據

### 代表性 EES 技術關鍵指標對比（摘自原論文 Tables 10–12）
> **工況與口徑註記**：下表效率、壽命與成本區間係原論文彙整 266 篇文獻之**多研究綜合區間**（非單一測試平台標準工況）；成本保留原文幣別（2015 年時點之 USD / EUR）。

| 技術 | 功率規模（MW） | 循環效率（%） | 循環壽命（cycles） | 響應時間 | 功率成本（$/kW） | 能量成本（$/kWh） | 成熟度 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **PHS** | `100–5,000` | `70–85`（最高 `87`） | `10,000–30,000` | 分鐘級 | `2,000–4,300` | `5–100` | 成熟（Mature） |
| **大型 CAES** | 最高 `300–1,000` | `42–54`（AA-CAES `~70`） | `8,000–12,000` | 分鐘級 | `400–1,000` | `2–120` | 商用 / AA-CAES 開發中 |
| **飛輪（FES）** | `0.1–20` | `90–95` | `20,000+` | 秒級 / `<1 cycle` | `250–350` | `1,000–14,000` | 早期商用 |
| **鉛酸電池** | `0–40` | `70–80`（`63–90`） | `500–2,000` | 毫秒級 | `200–600` | `50–600` | 成熟 |
| **鋰離子電池** | `0.005–100` | `75–97` | `1,000–10,000`（最高 `20,000`） | 毫秒級 | `900–4,000` | `600–3,800` | 示範（2015 時點） |
| **鈉硫電池（NaS）** | `< 34–40` | `75–90` | `2,500–4,500` | 原文未提供 | `350–3,000` | `300–500` | 商用 |
| **全釩液流（VRB）** | `0.03–3`（潛力 `50`） | `65–85` | `10,000–16,000+` | `< 0.001 s` | `600–1,500` | `150–1,000` | 示範 / 早期商用 |
| **超級電容（EDLC）** | `0–0.3+` | `84–97` | `100,000+` | 毫秒級 | `100–450` | `300–2,000`（文中 `>6,000`） | 開發 / 示範 |
| **SMES** | `0.1–10` | `95–98` | `100,000+` | 毫秒級 | `200–489`（文中至 `7,200`） | `500–72,000` | 示範 / 早期商用 |
| **氫氣燃料電池** | `< 50`（至 `58.8`） | `20–50`（最高 `66`） | `1,000–20,000+` | 秒級 | `500–3,000` | `15`（`2–15 €/kWh`） | 開發 / 示範 |
| **液態空氣（LAES）** | `10–200` | `55–80+` | 原文未提供（日曆壽命 `25+ yr`） | 分鐘級 | `900–1,900` | `260–530` | 開發 / 示範 |

### 指標實場案例
- **PHS**：美國 Bath County（`3,003 MW`，全球最大）；日本沖繩 Yanbaru（`~30 MW / 180 MWh`，唯一商用海水抽蓄）。
- **CAES**：德國 Huntorf（1978，`290 MW / 580 MWh`，效率 `~42%`）；美國 McIntosh（1991，`110 MW / 2,860 MWh`，回熱器省燃料 `22–25%`，效率 `~54%`）；德國 ADELE 無碳絕熱 AA-CAES 示範（`90 MW / 360 MWh`，目標效率 `~70%`）。
- **電化學與飛輪**：日本 Rokkasho 風電配 NaS（`34 MW / 244.8 MWh`）；美國 AES Laurel Mountain 風電配鋰電（`32 MW / 8 MWh`）；紐約 Beacon Power 飛輪調頻（`20 MW / 5 MWh`，供應紐約州約 `10%` 調頻服務）。

---

## 5. 假設條件、工程限制與未解問題

1. **地質與地理約束**：PHS 受限於地形水文與漫長工期；CAES 高度依賴地下鹽穴或地質構造（美國愛荷華 `270 MW` 砂岩含水層案因流率不足於 2011 年取消；義大利 Sesta `25 MW` 案因地熱擾動中止）。
2. **壽命、維運與自放電取捨**：低能量成本不等於低全生命週期成本（鉛酸電池循環壽命僅 `500–2,000` 次、O&M 約 `50 $/kW/yr`）；NaS 需維持 `574–624 K`（O&M `~80 $/kW/yr`）；飛輪、超級電容與 SMES 自放電率極高，無法勝任長時備用。
3. **季節性儲能商業空白**：電化學與機械儲能無法低成本跨越數週至數月尺度，仍須依賴化學燃料（氫能或 [[Power-to-Gas and Methanation Processes|合成天然氣 SNG]]）。

---

## 6. 知識庫關聯與觀點衝突

- **核心概念**：[[Electrical Energy Storage (EES) Classification]]
- **跨領域延伸**：[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Hydrogen Storage Technologies and Metal Hydrides]]、[[Power-to-Gas and Methanation Processes]]
- **全五篇綜合比較**：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]

> [!warning] 觀點衝突 / 條件差異：單一儲能技術無法通吃全時間尺度與高效率
> - **短時高功率端（SMES / 超級電容 / 飛輪）**：往返效率高達 `90–98%`、毫秒級響應，但能量成本高達 `1,000–72,000 $/kWh` 且自放電嚴重。
> - **長時／季節端（氫氣燃料電池 / 太陽能燃料）**：能量成本低至 `2–15 €/kWh` 且自放電趨近於零，但電對電往返效率僅 `20–50%`；實務上需透過 Hybrid EES 或與 [[Power-to-Gas and Methanation Processes|Power-to-Gas]] 部門耦合來化解。
