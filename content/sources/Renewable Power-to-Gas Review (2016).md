---
type: source
title: "Renewable Power-to-Gas: A technological and economic review"
authors:
  - "Manuel Götz"
  - "Jonathan Lefebvre"
  - "Friedemann Mörs"
  - "Amy McDaniel Koch"
  - "Frank Graf"
  - "Siegfried Bajohr"
  - "Rainer Reimert"
  - "Thomas Kolb"
year: 2016
venue: "Renewable Energy, Vol. 85, pp. 1371–1390"
doi: "10.1016/j.renene.2015.07.066"
raw_file: "raw/papers/Renewable Power-to-Gas A technological and economic review.pdf"
status: ingested
tags:
  - source
  - power-to-gas
  - methanation
  - electrolysis
  - sector-coupling
  - commercialization
aliases:
  - "Götz et al. (2016) Power-to-Gas Review"
  - "再生能源電轉氣技術與經濟綜述 (2016)"
updated: 2026-11-21
---

# Renewable Power-to-Gas Review (2016)

> **原始論文**：`raw/papers/Renewable Power-to-Gas A technological and economic review.pdf`  
> **出處**：M. Götz et al., *Renewable Energy* 85 (2016) 1371–1390

---

## 1. 核心貢獻（TL;DR）

1. **端對端 Power-to-Methane（SNG）全鏈條評估**：系統檢視「電解產氫 → 暫時性儲氫 → $\text{CO}_2$ 捕集／碳源 → 催化／生物甲烷化 → 併入天然氣管網」各環節，量化無廢熱整合下全鏈效率約 **`55%`**（電解 `70%` × 甲烷化 `78%`）。
2. **三大電解槽動態與成本基準**：指出 [[Water Electrolysis Technologies (AEL, PEM, SOEC)|鹼性電解（AEL）]] 目前最成熟便宜（`~1,000 €/kW`，系統壽命達 `30 yr`）；質子交換膜（PEMEL）動態響應最佳（最低負載 `5%`、冷啟動秒至分鐘級），最適合未來間歇性再生能源；固態氧化物（SOEC）吸熱模式理論電效率可 `> 100%`，但仍處實驗室階段。
3. **催化 vs. 生物甲烷化工程分野**：量化催化甲烷化空速（GHSV `2,000–5,000 h⁻¹`）高出生物甲烷化（實際 `< 10 h⁻¹`）逾兩個數量級且具高溫廢熱回收價值（`≥ 300 °C`）；生物甲烷化雖耐硫／耐雜質，但受限於 $\text{H}_2$ 氣液傳質與攪拌能耗（佔 SNG 能量 `~10%`），在 `110 MW` 規模下成本高達催化的 `2.5` 倍，僅適合小型沼氣廠。
4. **經濟性現實與商業模式突圍**：彙整文獻 SNG 生產成本（`4–90 ct/kWh`，視滿載時數 FLH 與電價而定），對比天然氣（`2–3 ct/kWh`）與生質甲烷（`~7 ct/kWh`），點出「高 FLH vs. 低電價」的根本經濟矛盾，主張結合車用燃料、電網平衡服務、碳權與延緩電網擴建之宏觀價值。

---

## 2. 研究背景與工程痛點

- 高比例再生能源（如 2013 年丹麥風電佔比 `34%`、西班牙 `21%`、德國 `9%`；德國剩餘負載達 `30–60 GW`）需要跨季節大規模儲能。
- 直接將 $\text{H}_2$ 注入現有天然氣管網受各國法規限制於 **`0–12 vol.%`**；轉化為合成天然氣（SNG, $\text{CH}_4$）則可無縫接入全球超過 **`3,600 TWh`** 的既有地下天然氣儲氣庫與管網（對照 2012 年全球風光總發電量 `639 TWh`），直接解決 [[Overview of Electrical Energy Storage Technologies (2015)|Luo et al. (2015)]] 所指出的季節性儲能空白。

---

## 3. 系統模型、拓撲與控制方法

### 核心電化學與熱化學反應式
1. **水電解總反應**：
   $$\text{H}_2\text{O(l)} \rightarrow \text{H}_2\text{(g)} + \frac{1}{2}\text{O}_2\text{(g)} \qquad \Delta H_r^0 = +285.8\ \text{kJ/mol}, \quad \Delta G_r^0 = n F E_V^0 = +237.1\ \text{kJ/mol}$$
2. **$\text{CO}_2$ 甲烷化（Sabatier 反應，強放熱）**：
   $$\text{CO}_2\text{(g)} + 4\text{H}_2\text{(g)} \rightleftharpoons \text{CH}_4\text{(g)} + 2\text{H}_2\text{O(g)} \qquad \Delta H_r^0 = -165.1\ \text{kJ/mol}$$
3. **$\text{CO}$ 甲烷化**：
   $$\text{CO(g)} + 3\text{H}_2\text{(g)} \rightleftharpoons \text{CH}_4\text{(g)} + \text{H}_2\text{O(g)} \qquad \Delta H_r^0 = -206.3\ \text{kJ/mol}$$
4. **逆水煤氣變換（RWGS）與 Boudouard 積碳反應**：
   $$\text{CO}_2 + \text{H}_2 \rightleftharpoons \text{CO} + \text{H}_2\text{O} \quad (\Delta H_r^0 = +41.2\ \text{kJ/mol}); \qquad 2\text{CO} \rightleftharpoons \text{C(s)} + \text{CO}_2 \quad (\Delta H_r^0 = -172.5\ \text{kJ/mol})$$
5. **反應器效能指標與氣液傳質**：
   $$\text{GHSV} = \frac{F_{V,G,\text{in}}}{V_R}, \qquad \text{MFR} = \frac{F_{V,\text{CH}_4,\text{out}} - F_{V,\text{CH}_4,\text{in}}}{V_R}, \qquad r_{i,\text{eff}} = (k_L a)_i \left(\frac{p_i \rho_L}{H_{i,L}} - c_{i,L}\right)$$

### 符號與 SI 單位對照表

| 符號 | 物理意義 | 單位 | 代表數值與工況 |
| --- | --- | --- | --- |
| $E_V^0$ | 平衡電池電壓 | `V` | AEL `1.8–2.4 V`；PEM `1.8–2.2 V`；SOEC `0.91–1.3 V` |
| $\text{GHSV}$ | 氣體時空速度 | `h⁻¹` | 絕熱固定床 `2,000–5,000`；三相漿態床 `500–1,000`；生物法 `< 10` |
| $\text{MFR}$ | 甲烷生成速率 | `h⁻¹` | 生物原位消化槽 `< 0.1`；獨立 CSTR `1.4–28.7` |
| $^V H_{i,\text{H}_2\text{O}}$ | 亨利溶解度常數（`60 °C`） | `bar·L/mol` | $\text{H}_2$: `1,408` vs. $\text{CO}_2$: `36`（$\text{H}_2$ 難溶為生物法傳質瓶頸） |
| $q'''_{\text{cat}}$ | 催化床體積放熱率 | `MW/m³` | $\text{GHSV} = 5,000\ \text{h}^{-1}$ 完全轉化時約 **`2 MW/m³`** |

---

## 4. 測試系統、工況條件與關鍵實驗／模擬數據

- **規模配比（假設電解能耗 `5 kWh/m³ H2`）**：
  - 沼氣廠（`500 m³/h CO2 + 500 m³/h CH4`）需 `10 MW` 電解 → 產 `11 MW` $\text{CH}_4$。
  - 生質氣化（BtG+PtG）結合 `59.5 MW` 電解 → 碳利用率翻倍以上（$\text{CH}_4$ 由 `2,700` 增至 `5,700 m³/h`，`63 MW`）。
  - 工業點源（`30,000 m³/h CO2`）需 `600 MW` 電解；大型電廠煙道氣（`300,000 m³/h CO2`）需高達 `6,000 MW` 電解。
- **動態甲烷化節省儲氫投資（`36 MW` 風電 PtG 案例，儲氫 `30–200 bar`）**：甲烷化採 `40–100%` 動態操作時，雖甲烷化投資由 `0.7` 增至 `1.2 M€`，但 $\text{H}_2$ 儲槽體積減半（`1,700 → 850 m³`）、儲氫投資由 `8.3` 降至 `4.8 M€`，**總 CAPEX 下降 `8%`（`38.8 → 35.8 M€`）**。
- **SNG 生產成本與敏感度**：
  - `1,200 h/a`（FLH）：`10–60 ct/kWh`（褐煤電廠整合達 `60–90 ct/kWh`）；`3,000 h/a`：`4–21 ct/kWh`（FLH 由 `1,200` 增至 `3,000 h/a` 可降本約 **`50%`**）。
  - 副產 $\text{O}_2$（`8 kg O2 / kg H2`）若以 `10–70 €/t` 售出可降本 `1.3–2 ct/kWh`；$\text{CO}_2$ 成本每 `100 €/t` 則增本 `2 ct/kWh`。
- **代表實場示範廠**：德國 Werlte **Audi e-gas**（2013，`6 MW el.` AEL + 沼氣 $\text{CO}_2$ + 冷卻固定床，論文發表時全球最大）；日本東北工業大學（2003，首座 `<10 kW` 試驗）；歐盟 **DemoSNG**（2015，蜂巢結構反應器 + 生質氣化）；丹麥 **BioCatProject**（`1 MW` AEL + 生物甲烷化）。

---

## 5. 假設條件、工程限制與未解問題

1. **滿載時數（FLH）與電價悖論**：攤提昂貴電解 CAPEX（`800–3,000 €/kW`）需要高 FLH，但僅依賴廉價棄風棄光剩餘電力的 FLH 偏低，兩者本質衝突。
2. **副產氧氣尚未商業化利用**：儘管每公斤氫伴隨 `8 kg` 高純度 $\text{O}_2$，因液化輸送成本高且間歇供應，當時尚無 PtG 示範廠成功變現。
3. **熱整合的經濟爭議**：將 SOEC 與放熱甲烷化耦合雖能拉高電效率，但文獻（Buttler et al.）指出用於間歇性電網儲能時會增加電池面積與 CAPEX，反而不具經濟效益。

---

## 6. 知識庫關聯與觀點衝突

- **核心方法**：[[Water Electrolysis Technologies (AEL, PEM, SOEC)]]、[[Power-to-Gas and Methanation Processes]]、[[Hydrogen Storage Technologies and Metal Hydrides]]
- **全五篇綜合比較**：[[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]

> [!warning] 觀點衝突 / 條件差異：催化甲烷化 CAPEX 估算落差達一個數量級
> - **工程報價（Outotec GmbH, 2014，作者評為最寫實）**：`20 bar` 催化甲烷化在 `5 MW` 為 `400 €/kW SNG`，`110 MW` 規模可降至 `130 €/kW SNG`。
> - **系統研究文獻（如 E&E Consultant 等）**：常引用 `500–1,500 €/kW SNG`，作者指出多數系統研究高估了催化甲烷化投資成本（真正主導總投資的是電解槽與暫存儲氫槽）。
