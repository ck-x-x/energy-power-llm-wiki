---
type: method
category: "sector-coupling"
tags:
  - method
  - power-to-gas
  - methanation
  - seasonal-storage
  - carbon-capture-utilization
aliases:
  - "電轉氣與甲烷化製程"
  - "Power-to-Methane (PtG)"
sources_count: 1
updated: 2026-11-21
---

# Power-to-Gas and Methanation Processes

Power-to-Gas（PtG / Power-to-Methane）將再生電力經 [[Water Electrolysis Technologies (AEL, PEM, SOEC)|水電解]] 轉為 $\text{H}_2$，再與 $\text{CO}_2$ 經甲烷化反應合成**合成天然氣（SNG, $\text{CH}_4$）**，突破天然氣管網僅允許 `0–12 vol.%` 摻氫的法規上限，直接接入全球逾 **`3,600 TWh`** 的既有天然氣儲運設施，成為跨季節儲能的關鍵解方 [[Renewable Power-to-Gas Review (2016)]]。

---

## 1. 全鏈條效率與碳源選擇

- **基準全鏈效率（無廢熱整合）**：**`55%`** = 電解（`70%`, `25 bar`）× 甲烷化（`78%`, `20 bar`）；若 $\text{CO}_2$ 需額外壓縮至 `20 bar`，效率再扣 `2%`。
- **近期至中期最佳碳源**：
  1. **沼氣廠（Biogas Plants）**：`30–50% CO2`，歐洲具約 `15,000` 座未併網沼氣廠，純化成本低且可就地消化廢熱與副產 $\text{O}_2$（典型 `10 MW` 電解配對）。
  2. **生質氣化整合（BtG + PtG）**：導入電解 $\text{H}_2$ 可省去水煤氣變換（WGS），使碳利用率**翻倍以上**（$\text{CH}_4$ 產出由 `2,700` 增至 `5,700 m³/h`），並利用副產 $\text{O}_2$ 氣化、大幅提升甲烷化滿載時數（FLH）。
  3. **大型工業／電廠煙道氣**：需昂貴捕集與深度脫硫，且單一電廠對應電解規模高達 **`6,000 MW`**，短期不具工程經濟性。

---

## 2. 催化甲烷化 vs. 生物甲烷化對比

核心 Sabatier 反應（強放熱，$\text{GHSV} = 5,000\ \text{h}^{-1}$ 時每立方公尺觸媒床釋放 **`~2 MW`** 熱量）：
$$\text{CO}_2\text{(g)} + 4\text{H}_2\text{(g)} \rightleftharpoons \text{CH}_4\text{(g)} + 2\text{H}_2\text{O(g)} \qquad \Delta H_r^0 = -165.1\ \text{kJ/mol}$$

為達 `> 90%` 乾基 $\text{CH}_4$（`≥ 98%` $\text{CO}_2$ 轉化率），熱力學要求於 `1 bar` 下操作溫度 `< 225 °C`，或於 `20 bar` 下 `< 300 °C`。

| 比較項目 | 催化：絕熱固定床（Fixed-Bed） | 催化：三相漿態床（3PM Slurry） | 生物甲烷化（BM, 獨立 CSTR） |
| --- | --- | --- | --- |
| **操作溫壓** | `300–550 °C`、`> 5 bar`（`2–6` 段冷卻） | `300–350 °C`、`~20 bar`（等溫） | `20–70 °C`、`< 10 bar` |
| **氣體時空速度（GHSV）** | **`2,000–5,000 h⁻¹`** | `500–1,000 h⁻¹` | `≪ 100 h⁻¹`（實際 **`< 10 h⁻¹`**） |
| **耐雜質（$\text{H}_2\text{S}$ 等）** | 極低（Ni 觸媒要求硫 `≪ 1 ppm`） | 低至中 | **高**（甲烷古菌耐 $\text{H}_2\text{S}$、$\text{O}_2$） |
| **動態與最低負載** | 商用約 `40%`；停機需 $\text{H}_2$ 吹掃並保溫 `> 200 °C` 防羰基鎳 | `25–100%` 變載維持等溫（高液相熱容） | 可 `100% → 0%` 瞬停，但攪拌耗能佔 SNG 能量 `~10%` |
| **廢熱品質與建議規模** | 極高（高溫蒸汽／發電），適合 **`> 100 MW`** | 佳至極佳，適合中型廠 | 差（`< 70 °C`），**僅適合小型廠**（`110 MW` 成本為催化 `2.5×`） |

---

## 3. 經濟性瓶頸與系統優化方向

- **SNG 成本區間**：`4–90 ct/kWh`（對照天然氣 `2–3 ct/kWh`、生質甲烷 `~7 ct/kWh`）；**滿載時數（FLH）從 `1,200` 提升至 `3,000 h/a` 可直接降本約 `50%`**。
- **動態甲烷化壓低儲氫 CAPEX**：在 `36 MW` 風電 PtG 案例中，以 `40–100%` 動態甲烷化取代穩態操作，可將暫存 $\text{H}_2$ 儲槽容積減半（`1,700 → 850 m³`）、整體總 CAPEX 下降 **`8%`**（`38.8 → 35.8 M€`）。
- **代表實場示範**：德國 Werlte **Audi e-gas**（`6 MW el.` AEL + 沼氣 $\text{CO}_2$）、歐盟 **DemoSNG**（蜂巢反應器 + 生質氣化）、丹麥 **BioCatProject**（`1 MW` 生物甲烷化）。

---

## 4. 相關知識庫連結
- 來源文獻：[[Renewable Power-to-Gas Review (2016)]]
- 上下游連結：[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Hydrogen Storage Technologies and Metal Hydrides]]、[[Electrical Energy Storage (EES) Classification]]
- 全五篇綜合比較：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]
