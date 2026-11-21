---
type: method
category: "extraction-and-sequestration"
tags:
  - method
  - natural-gas-hydrates
  - co2-sequestration
  - carbon-neutral
  - guest-exchange
aliases:
  - "CH4-CO2 置換法"
  - "二氧化碳置換開採"
  - "CO2-CH4 Guest Exchange"
sources_count: 1
updated: 2026-11-21
---

# CH4-CO2 Hydrate Exchange Process

$\text{CH}_4$–$\text{CO}_2$ 客體置換法是將 $\text{CO}_2$（或含 $\text{CO}_2$ 煙道氣）注入 [[Natural Gas Hydrates (NGH)|天然氣水合物]] 儲層，在釋放 $\text{CH}_4$ 的同時將 $\text{CO}_2$ 以固態水合物形式永久封存於地層的雙贏技術 [[Review of Natural Gas Hydrates as an Energy Resource (2016)]]。

---

## 1. 熱力學驅動力與四大潛在優勢

1. **相平衡穩定度優勢**：$\text{CO}_2$ 分子直徑（`5.12 Å`）大於 $\text{CH}_4$（`4.36 Å`），兩者皆主要形成 sI 水合物；但在低溫區（`< 10 °C`），$\text{CO}_2$ 水合物相平衡壓力低於 $\text{CH}_4$ 水合物（更穩定）。於 `280 K` 混合系統中，氣相／水合物相分佈係數比 $(y/z)_{\text{CH}_4} / (y/z)_{\text{CO}_2} = 2.5$，證實 $\text{CO}_2$ 偏好進入水合物晶格。
2. **熱量自持（Self-Sustainable Heat Balance）**：
   $$\Delta H_{\text{CO}_2,\text{form}} = -57.98\ \text{kJ/mol}, \qquad \Delta H_{\text{CH}_4,\text{diss}} = +54.49\ \text{kJ/mol}$$
   $\text{CO}_2$ 水合物生成釋放的熱量大於 $\text{CH}_4$ 水合物分解所需吸熱，理論上可大幅減少外部供熱需求。
3. **碳中和能源循環**：若地層封存的 $\text{CO}_2$ 摩爾量等於或大於產出 $\text{CH}_4$ 燃燒產生的 $\text{CO}_2$，整體發電與開採鏈可趨近碳中和；且直接注入煙道氣（Flue Gas）可省去昂貴的 $\text{CO}_2$ 濃縮捕集成本（參考：燃煤電廠捕集成本 `US$ 50–75 / t CO2 avoided`，IGCC 約 `US$ 35–46 / t CO2 avoided`）。
4. **減產水與穩固海床**：分解釋放的水隨即參與 $\text{CO}_2$ 水合物生成（Bentheim 砂岩 MRI 實驗未見明顯自由水產出），且新生成的 $\text{CO}_2$ 水合物可替代原骨架維持 [[Hydrate-Bearing Sediment Geomechanics|海床機械穩定性]]。

> [!warning] 觀點衝突 / 條件差異：理想模擬 vs. 真實儲層的熱力學與動力學落差
> - **理想分子動力學（MD）**：Yezdimer et al. (2002) 在純水、純氣、完全飽和水合物條件下計算置換吉布斯自由能 $\Delta G \approx -12\ \text{kJ/mol}$，證明熱力學自發。
> - **實地非理想條件與 sII 混合氣**：真實儲層含多孔介質、鹽水與非完全飽和狀態；且若天然氣含 `0.5 mol%` 丙烷形成 sII 水合物，其穩定度大幅逼近 $\text{CO}_2$ 水合物。不過 Raman / PXRD 研究顯示，透過營造富 $\text{CO}_2$ 氣相造成的**化學非平衡（Chemical Disequilibrium）**仍可於 `10 h` 內驅動置換。

---

## 2. 不同注入型態與儲層條件之實驗表現

NMR 微觀佔位研究顯示，基於大籠完全佔據（$\theta_L = 1$）與稀釋態小籠平衡比（$\theta_L / \theta_S = 0.23$），純 sI 水合物中 $\text{CO}_2$ 難以進入小籠（約 `1/3` 會被 $\text{CH}_4$ 再佔據），推導出理論最低甲烷回收率為 **`64%`**（水合物相 $\text{CO}_2/\text{CH}_4 = 1.8$）。然而，實際實驗回收率普遍偏低（未加熱系統多 **`< 40%`**）：

| 注入介質／工況 | 儲層／樣品條件 | 反應時間 | $\text{CH}_4$ 回收率 | 關鍵機制與限制 |
| --- | --- | --- | --- | --- |
| 液態 $\text{CO}_2$（早期塊體） | 純水塊體，`274–277 K, 4–5 MPa` | `> 800 h` | `~12.5%` | 介面形成 $\text{CO}_2$ 水合物外殼阻斷傳質 |
| 氣態 $\text{CO}_2$（細粉冰） | `5–50 μm` 細粒水合物（具體溫壓原文未提供） | `< 5 h` | `~50%` | 粒徑增至 `1 mm` 時回收率暴跌逾 `3` 倍 |
| 氣態 vs. 液態 $\text{CO}_2$（7 L 釜） | `3.35 wt.% Na2SO4` + 20–40 mesh 石英砂（孔隙率 `38.7%`） | 原文未提供 | 液態最高 `35%` | 液態 $\text{CO}_2$ 逸度降幅小，於 Class I–III 皆優於氣態；氣態僅在 **Class I** 顯著有效 |
| $\text{CO}_2$/水乳液（C/W Emulsion） | 石英砂 + SDS，`281.2 K, 5 MPa` | 原文未提供 | 速率高於液態 $\text{CO}_2$ | 改善多相流熱質傳遞，最佳策略為「先降壓再注乳液」，但乳液製備具技術門檻 |
| 超臨界 $\text{CO}_2$（`95 °C` 階梯注入） | 石英砂 + 冰粒，`2–10 °C, 8–13 MPa` | `44 h` | `40.7%` | 雙穩定區會快速生成 $\text{CO}_2$ 堵塞流道；分解區則出現熱流竄流（Channelling） |
| 液態 $\text{CO}_2$（固結砂岩 MRI） | Bentheim 砂岩岩心 + `0.1 wt.% NaCl`（具體溫壓原文未提供） | 原文未提供 | `50–60%` | 固結剛性砂岩孔隙表現遠優於未固結散砂，且無明顯自由水產出 |

---

## 3. 五大關鍵影響因子與未解瓶頸

1. **水合物粒徑**：粒徑由 `5–50 μm` 增至 `1 mm`，回收率下降逾 `3` 倍。
2. **固相擴散阻礙層（主瓶頸）**：表面先形成混合水合物殼層向內收縮，固相擴散極慢——水合物中 $D_{\text{CO}_2} = 1 \times 10^{-12}\ \text{m}^2/\text{s}$ (`273 K`) 至 $1 \times 10^{-23}\ \text{m}^2/\text{s}$ (`200 K`)；$D_{\text{CH}_4} = 3.4\text{–}7.6 \times 10^{-13}\ \text{m}^2/\text{s}$ (`3–15 MPa, 263–268 K`)。Raman 動力學模型求得 $\text{CH}_4$ 分解活化能 `14.5 kJ/mol`、$\text{CO}_2$ 生成活化能 `73.3 kJ/mol`，確認受固相傳質控制。
3. **客體超額逸度（Excess Fugacity）**：液態 $\text{CO}_2$ 逸度衰減小於氣態，驅動力更持久。
4. **多孔介質性質**：固結砂岩（`50–60%`）與未固結散砂（多 `< 40%`）差異顯著。
5. **最佳溫壓操作窗**：位於 $\text{CH}_4$ 水合物不穩定、而 $\text{CO}_2$ 水合物穩定的三曲線夾角區（`L_CO2–V_CO2`、`H–L_w–L_CO2`、`H–L_w–V–CH4`），並已在 [[NGH Field Trials and Commercialization Comparison|Ignik Sikumi 2012 現場試驗]] 獲得實場固相置換驗證。

---

## 4. 相關知識庫連結
- 來源文獻：[[Review of Natural Gas Hydrates as an Energy Resource (2016)]]
- 相關概念：[[Natural Gas Hydrates (NGH)]]、[[Hydrate-Bearing Sediment Geomechanics]]
- 對比方法：[[Conventional NGH Dissociation Methods]]
- 實場與經濟：[[NGH Field Trials and Commercialization Comparison]]
