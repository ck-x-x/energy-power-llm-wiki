---
type: concept
tags:
  - concept
  - electrical-energy-storage
  - power-systems
  - grid-services
aliases:
  - "電能儲存分類與電網應用"
  - "EES 六大分類"
sources_count: 1
updated: 2026-11-21
---

# Electrical Energy Storage (EES) Classification

電能儲存（Electrical Energy Storage, EES）將電網多餘電能轉換為可儲存的能量型態，並於尖峰或暫態擾動時釋放回電網。依儲存能量型態可劃分為**六大類別**，並對應電力系統三大時間尺度應用 [[Overview of Electrical Energy Storage Technologies (2015)]]。

---

## 1. 六大儲能分類與代表技術

1. **機械儲能（Mechanical）**：抽蓄水力（PHS，`100–5,000 MW`，佔 2012 全球大型儲能 `> 99%`）、壓縮空氣（CAES，`110–300+ MW`；無碳絕熱 AA-CAES 目標效率 `~70%`）、飛輪（FES，高速碳纖轉子達 `10⁵ rpm`、`~100 Wh/kg`）。
2. **電化學儲能（Electrochemical）**：
   - 傳統二次電池：鉛酸（`2.0 V`）、鋰離子（`3.7 V`，`75–97%`）、鈉硫 NaS（`574–624 K`，`~2.08 V`）、鎳鎘 NiCd、ZEBRA（`523–623 K`）。
   - 液流電池（FBES，功率與能量解耦）：全釩 VRB（`~1.4 V`，`10,000–16,000+` 次循環）、鋅溴 ZnBr（`1.8 V`）、多硫化鈉溴 PSB。
3. **電氣儲能（Electrical）**：電容器、超級電容 EDLC（`100,000+` 次循環、`84–97%`）、超導磁儲能 SMES（LTS `~5 K` / HTS `~70 K`，`95–98%`、功率密度高達 `4,000 W/L`）。
4. **熱化學儲能（Thermochemical）**：太陽能燃料（自然／人工光合作用、聚光熱化學裂解水，比能量 `800–100,000 Wh/kg`，效率 `~20–30%`）。
5. **化學儲能（Chemical）**：[[Water Electrolysis Technologies (AEL, PEM, SOEC)|電解產氫]] + [[Hydrogen Storage Technologies and Metal Hydrides|儲氫]] + 燃料電池（AFC / PAFC / SOFC / MCFC / PEMFC / DMFC；往返效率 `20–50%`、能量成本僅 `2–15 €/kWh`）。
6. **熱能儲能（Thermal, TES）**：低溫含水層／冰蓄冷、低溫液態空氣儲能（LAES，`214 Wh/kg`，能量密度為 `200 bar` CAES 的 `4–6` 倍）、高溫熔鹽／相變材料／混凝土儲熱。

---

## 2. 電力系統三大時間尺度與應用配對

| 電網服務層級 | 功率範圍 | 響應時間 | 放電時長 | 已實證技術（Experienced） | 具潛力技術（Promising） |
| --- | --- | --- | --- | --- | --- |
| **電能品質（Power Quality / LVRT）** | `< 1 MW`（輸配穩態至 `100 MW`） | 毫秒級（`< 1/4 cycle`） | `ms–s` | 飛輪、電池、SMES、超級電容 | 液流電池 |
| **橋接／穿越電源（Bridging / Smoothing）** | `100 kW–20 MW` | `≤ 1 s` | `s–min`（至小時） | 電池、液流電池、飛輪、超級電容 | 燃料電池、SMES |
| **能量管理（Time Shifting / Peak Shaving）** | `1–500+ MW` | 分鐘級 | `3–24 h+` | 大型：PHS、CAES、TES；中小型：電池、液流電池 | 燃料電池、太陽能燃料 |
| **季節性儲能（Seasonal Storage）** | `30–500 MW` | 分鐘級 | 數週至數月 | **尚無商業化技術** | PHS、TES、燃料電池；以及 [[Power-to-Gas and Methanation Processes|Power-to-Gas（SNG）]] |

---

## 3. 相關知識庫連結
- 來源文獻：[[Overview of Electrical Energy Storage Technologies (2015)]]
- 銜接季節儲能：[[Power-to-Gas and Methanation Processes]]、[[Hydrogen Storage Technologies and Metal Hydrides]]
- 全五篇綜合比較：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]
