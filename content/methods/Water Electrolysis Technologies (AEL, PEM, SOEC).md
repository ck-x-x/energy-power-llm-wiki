---
type: method
category: "electrochemical-conversion"
tags:
  - method
  - electrolysis
  - hydrogen-production
  - power-to-gas
aliases:
  - "水電解技術比較 (AEL / PEM / SOEC)"
  - "電解產氫技術"
sources_count: 2
updated: 2026-11-21
---

# Water Electrolysis Technologies (AEL, PEM, SOEC)

水電解是連結再生電力、[[Hydrogen Storage Technologies and Metal Hydrides|氫能儲運]] 與 [[Power-to-Gas and Methanation Processes|Power-to-Gas]] 的核心電化學樞紐，但截至 2016–2020 年僅佔全球總產氫量的 **`4–5%`** [[Hydrogen Production for Energy Overview (2020)]] [[Renewable Power-to-Gas Review (2016)]]。

---

## 1. 電化學反應與熱力學基礎

$$\text{H}_2\text{O(l)} \rightarrow \text{H}_2\text{(g)} + \frac{1}{2}\text{O}_2\text{(g)} \qquad \Delta H_r^0 = +285.8\ \text{kJ/mol}, \quad \Delta G_r^0 = n F E_V^0 = +237.1\ \text{kJ/mol}$$

- **溫壓效應**：提高溫度會降低平衡電壓 $E_V$（減少電能需求、增加熱能需求）；提高壓力會略增 $E_V$（微降電效率），但加壓電解所省下的下游壓縮能耗大於電效率折損 [[Renewable Power-to-Gas Review (2016)]]。
- **副產氧氣**：每產 `1 kg H2` 伴隨 `8 kg O2`（對應 $\text{CO}_2$ 甲烷化約 `2 m³ O2 / m³ CH4`）。

---

## 2. 三大水電解槽綜合基準對比

綜合 Götz et al. (2016) 與 Dawood et al. (2020) 之技術經濟數據：

| 比較項目 | 鹼性電解（AEL / AE） | 質子交換膜電解（PEMEL / PEM） | 固態氧化物電解（SOEC / SOC） |
| --- | --- | --- | --- |
| **電解質與載流子** | `20–30%` KOH/NaOH 水溶液（$\text{OH}^-$） | 固態高分子膜 Nafion（$\text{H}_3\text{O}^+/\text{H}^+$） | `8 mol% Y2O3` 摻雜 $\text{ZrO}_2$ 陶瓷（$\text{O}^{2-}$） |
| **操作溫度 / 電壓** | `40–90 °C` / `1.8–2.4 V` | `20–100 °C` / `1.8–2.2 V` | `800–1,000 °C` / `0.91–1.3 V` |
| **系統效率（Dawood 2020）** | `62–82%`（TML `9–10`） | `67–84%`（TML `7–9`） | `75–90%`（TML `3–5`；吸熱模式理論電效率 `> 100%`） |
| **系統能耗（Götz 2016, $H_S$）** | 現況 `4.5–8.2` → 未來 `4.3–5.7 kWh/m³ H2` | 現況 `4.5–7.5` → 未來 `4.1–4.8 kWh/m³ H2` | 原文未提供系統能耗（實驗室階段） |
| **最低負載與動態響應** | `20–100%`（過載至 `150%`）；冷啟分鐘至小時（停機重啟 `30–60 min`） | **最低 `5%`**；冷啟**秒至分鐘級**，最適合間歇再生能源 | 不適合劇烈波動與間歇供電 |
| **壽命與翻修週期** | 電堆翻修 `7–12 yr`；系統壽命達 **`30 yr`** | 壽命約 `5 yr`（較 AEL 短） | 材料快速劣化、長期穩定度不足 |
| **單位建置成本（CAPEX）** | **`~1,000 €/kW`**（目前最便宜） | 2016 時約 `≥ 2× AEL`（預測 2018 `< 1,000 €/kW`、2020 `1,250 €/kW`） | 2016 估算高；預測 2030 達 `1,000 €/kW` |
| **單機規模（2016 時點）** | `< 760 m³/h`（`~2.7 MW`） | 最高 `~450 m³/h`（`~1.6 MW`） | 實驗室規模 |

---

## 3. 新興電解架構（Dawood et al., 2020）
> **工況註記**：以下四項新興架構之具體測試溫度、壓力與實驗室規模條件，**原文未提供**（摘自 Dawood et al., 2020 Table 5 綜合評述）。

- **陰離子交換膜（AEM）**：效率 `67–74%`，結合鹼性低成本觸媒與固態膜優勢。
- **無膜電解槽（Membraneless）**：效率 `40–80%`，研發聚焦加壓與放大。
- **Battolyser（電池 + 電解一體機）**：整體效率 **`76–90%`**，同時提供短時充放電與產氫。
- **一體化再生燃料電池（URFC）**：電對電往返效率 **`43–51%`**。

> [!warning] 觀點衝突 / 條件差異：水電解效率口徑差異（Götz 2016 vs. Dawood 2020）
> - **[[Renewable Power-to-Gas Review (2016)]]**：採工業系統實務基準，將現行 AEL/PEM 系統電效率定於約 `70%`（`25 bar`），並指出 SOEC 在吸熱模式下計入外部高溫廢熱時**理論電效率可 `> 100%`**（但仍處實驗室階段）。
> - **[[Hydrogen Production for Energy Overview (2020)]]**：以總能量轉換效率區間列示 AE `62–82%`（TML `9–10`）、PEM `67–84%`（TML `7–9`）、SOEC `75–90%`（TML `3–5`）；兩者差異源於「純電效率（吸熱外熱計入分母與否）」與「多文獻文獻區間 vs. 單一系統基準值」之定義口徑不同。

---

## 4. 相關知識庫連結
- 來源文獻：[[Renewable Power-to-Gas Review (2016)]]、[[Hydrogen Production for Energy Overview (2020)]]
- 相關概念：[[Hydrogen Cleanness Index and Purity Standards]]
- 下游銜接：[[Hydrogen Storage Technologies and Metal Hydrides]]、[[Power-to-Gas and Methanation Processes]]
- 全五篇綜合比較：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]
