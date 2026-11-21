---
type: source
title: "Review of natural gas hydrates as an energy resource: Prospects and challenges"
authors:
  - "Zheng Rong Chong"
  - "She Hern Bryan Yang"
  - "Ponnivalavan Babu"
  - "Praveen Linga"
  - "Xiao-Sen Li"
year: 2016
venue: "Applied Energy, Vol. 162, pp. 1633–1652"
doi: "10.1016/j.apenergy.2014.12.061"
raw_file: "raw/papers/Review of natural gas hydrates as an energy resource Prospects.pdf"
status: ingested
tags:
  - source
  - natural-gas-hydrates
  - energy-resource
  - co2-sequestration
  - field-trials
  - commercialization
aliases:
  - "Chong et al. (2016) NGH Review"
  - "天然氣水合物能源綜述 (2016)"
updated: 2026-11-21
---

# Review of Natural Gas Hydrates as an Energy Resource (2016)

> **原始論文**：`raw/papers/Review of natural gas hydrates as an energy resource Prospects.pdf`  
> **出處**：Z. R. Chong, S. H. B. Yang, P. Babu, P. Linga, X.-S. Li, *Applied Energy* 162 (2016) 1633–1652

---

## 1. 核心貢獻（TL;DR）

1. **全球資源量收斂與可採性辨析**：梳理 1973–2014 年間的全球 [[Natural Gas Hydrates (NGH)|天然氣水合物（NGH）]] 資源估算演進——共識值由 1990 年代的 `20,000 TCM` 下修至近年的 `3,000 TCM`（Table 1 範圍 `1,000–5,000 TCM`，技術可採資源約 `300 TCM`），仍遠高於常規天然氣（`404 TCM`）與頁岩氣（`204–456 TCM`）；同時指出僅有高滲透率、高飽和度的**砂岩儲層（Sand Reservoirs）**具短期開採經濟性。
2. **系統評估四大開採技術與尺度瓶頸**：對比熱激法、降壓法、化學抑制劑注入與複合開採法（詳見 [[Conventional NGH Dissociation Methods]]），點出**實驗室尺度受限於傳熱（Heat Transfer），而實場大儲層受限於滲透率與流體流動（Flow Factors）**的關鍵尺度差異。
3. **深度解析 $\text{CH}_4$–$\text{CO}_2$ 置換與碳中和閉環**：系統回顧 [[CH4-CO2 Hydrate Exchange Process|$\text{CH}_4$–$\text{CO}_2$ 置換法]] 的熱力學自持優勢（$\text{CO}_2$ 生成放熱 `-57.98 kJ/mol` 大於 $\text{CH}_4$ 分解散熱 `+54.49 kJ/mol`），以及固相擴散層造成典型回收率低於 `40%` 的傳質瓶頸。
4. **全球現場試驗總結與商業化經濟門檻（本次共讀重點）**：彙整 Messoyakha、Mt. Elbert、Mallik、Ignik Sikumi 與 Nankai Trough 等實場試驗成果（詳見 [[NGH Field Trials and Commercialization Comparison]]），指出商業化前須達成 **`20,000–30,000 m³/d` 持續約 2 個月**的穩產測試，且突破關鍵在於**出砂管理（Sand Management）、產水處理、地質力學穩定性與環境風險控管**。

---

## 2. 研究背景與工程痛點

- **全球能源需求與碳排壓力**：依據 US DOE 2013 基準預測，全球能源消耗將由 2010 年的 `524 quadrillion BTU` 成長 `56%` 至 2040 年的 `820 quadrillion BTU`（非 OECD 國家以中國、印度為主成長 `112%`）。即便再生能源成長，2040 年仍有超過 `76%` 能源來自碳基燃料；其中天然氣單位能量 $\text{CO}_2$ 排放最低且年增速最快（`1.7%/yr`），成為取代煤炭的重要過渡能源。
- **與常規／頁岩氣開採的本質差異**：常規天然氣受致密蓋層封閉、頁岩氣受超低滲透率基質限制，開採核心在於建立導流通道（如水力壓裂）；但 NGH 的氣體分子是透過凡得瓦力（van der Waals forces）被鎖在水分子籠形晶格中，因此開採除了建立流道外，還必須進行**原位分解（In Situ Dissociation）**，且分解過程為**強吸熱反應**，易引發結冰、[[Self-Preservation Phenomenon|自我保護效應]] 與 [[Hydrate-Bearing Sediment Geomechanics|海床沉降／滑坡]]。

---

## 3. 系統模型、拓撲與控制方法

本篇為領域綜述論文，未提出單一全新控制律，而是統整水合物相平衡、熱傳、擴散與置換熱力學的核心物理關係：

### 3.1 關鍵物理與熱力學關係
- **$\text{CH}_4$–$\text{CO}_2$ 客體置換熱平衡**：
  $$\Delta H_{\text{CO}_2,\text{form}} = -57.98\ \text{kJ/mol}, \qquad \Delta H_{\text{CH}_4,\text{diss}} = +54.49\ \text{kJ/mol}$$
  $$\Delta G_{\text{exchange}} \approx -12\ \text{kJ/mol} \quad (\text{理想分子動力學模擬條件})$$
  由於 $\left|\Delta H_{\text{CO}_2,\text{form}}\right| > \Delta H_{\text{CH}_4,\text{diss}}$，理論上置換反應可達熱量自持。
- **氣水比（Gas-to-Water Ratio, $R_{\text{GW}}$）與氣體分佈係數**：
  - 氣水比 $R_{\text{GW}} = \dfrac{V_{\text{CH}_4,\text{STP}}}{V_{\text{water}}}$，在 117.8 L 中試規模（PHS）吞吐法（Huff-and-Puff）中實測 $R_{\text{GW}} > 55\ \text{m}^3\ \text{CH}_4\text{ (STP)}/\text{m}^3\ \text{water}$。
  - $\text{CH}_4$–$\text{CO}_2$ 混合水合物於 `280 K` 下之分佈係數比 $(y/z)_{\text{CH}_4} / (y/z)_{\text{CO}_2} = 2.5$，證實 $\text{CO}_2$ 傾向進入水合物固相、$\text{CH}_4$ 傾向釋放至氣相。

### 3.2 關鍵物理符號與 SI 單位對照表

| 符號 | 物理意義 | SI 單位（或原文常用單位） | 論文記載代表數值與條件 |
| --- | --- | --- | --- |
| $k$ | 熱導率（Thermal conductivity） | $\text{W/(m}\cdot\text{K)}$ | 純 $\text{CH}_4$ 水合物：`0.5–0.65`（水 `0.56` @ `0 °C`；冰 `2.14`） |
| $q''$ | 熱通量（Heat flux） | $\text{W/m}^2$ | 實驗室熱激測試範圍：`255–13,700` |
| $k_d$ | 水合物分解動力學常數 | $\text{mol}\cdot\text{m}^{-2}\cdot\text{Pa}^{-1}\cdot\text{s}^{-1}$ | `TOUGH-Fx/Hydrate` 擬合量級：$10^4$（`273–275 K`, `0.1–1.93 MPa`） |
| $D_{\text{CO}_2}$ | $\text{CO}_2$ 在水合物中之擴散係數 | $\text{m}^2/\text{s}$ | $1 \times 10^{-12}$ @ `273 K`；$1 \times 10^{-23}$ @ `200 K` |
| $D_{\text{CH}_4}$ | $\text{CH}_4$ 在 $\text{CH}_4$ 水合物中之擴散係數 | $\text{m}^2/\text{s}$ | $3.4 \times 10^{-13}$ 至 $7.6 \times 10^{-13}$（`3–15 MPa`, `263–268 K`） |
| $E_a$ | 活化能（Activation energy） | $\text{kJ/mol}$ | $\text{CH}_4$ 分解：`14.5`；$\text{CO}_2$ 生成：`73.3` |
| $\Delta T, \Delta P$ | 觸發分解之最小溫升／降壓驅動力 | $\text{K}$, $\text{MPa}$ | 海床工況（`4 °C, 8 MPa`）：$\Delta T \ge 7\ \text{K}$ 或 $\Delta P \ge 4.2\ \text{MPa}$ |
| $R_{\text{GW}}$ | 氣水比（Gas-to-water ratio） | $\text{m}^3\text{ (STP)}/\text{m}^3$ | PHS 吞吐法：`> 55`（`117.8 L`, `4.7 MPa` 起始壓力） |

---

## 4. 測試系統、工況條件與關鍵實驗／模擬數據

本綜述彙整之關鍵實場與經濟基準數據整理如下（完整解析請見 [[NGH Field Trials and Commercialization Comparison]]）：

### 4.1 全球 NGH 現場開採試驗總表（Table 2）

| 試驗場址 | 地點 | 年份 | 開採方法 | 產氣時間 | 累積產氣量（$\text{m}^3$） |
| --- | --- | --- | --- | --- | --- |
| Mt. Elbert Well | 美國阿拉斯加北坡 | 2007 | 降壓法（地層測試） | `11 h` | 原文未提供（`–`） |
| Mallik Site | 加拿大麥肯齊三角洲 | 2002 | 熱激法 | `5 days` | `516` |
| Mallik Site | 加拿大麥肯齊三角洲 | 2007 | 降壓法 | `12.5 h` | `830` |
| Mallik Site | 加拿大麥肯齊三角洲 | 2007–2008 | 降壓法 | `139 h`（6 days） | `13,000` |
| Ignik Sikumi | 美國阿拉斯加北坡 | 2012 | $\text{CO}_2/\text{CH}_4$ 置換（含 $\text{N}_2$ 煙道氣） | `~6 weeks` | `24,085`（`855 MSCF`） |
| Nankai Trough | 日本南海海槽（Daini Atsumi Knoll） | 2013 | 降壓法（全球首次海域試驗） | `6 days` | `120,000` |

### 4.2 資源量與生產成本對比（Table 1）
> **非 SI 單位換算註記**：`1 TCM` = $10^{12}\ \text{m}^3$；`1 Mbtu` $\approx 1.055\ \text{GJ} \approx 293.1\ \text{kWh}$；`1 MSCF` $\approx 28.32\ \text{m}^3\text{ (STP)}$；`1 Å` = $10^{-10}\ \text{m}$；`1 quadrillion BTU` $\approx 1.055\ \text{EJ}$。

| 天然氣來源 | 資源估算量（$\text{TCM}$） | 預估生產成本（$\text{USD/Mbtu}$） |
| --- | --- | --- |
| 常規天然氣（Conventional） | `404` | `2.00–9.00` / `0.53–6.02` |
| 緻密氣（Tight gas） | `84–210` | `3.00–8.00` / `2.75–8.03` |
| 頁岩氣（Shale gas） | `204–456` | `3.00–7.00` / `4.01–9.08` |
| 煤層氣（CBM） | `118–256` | `3.00–8.00` / `4.01–8.03` |
| 天然氣水合物（NGH） | `1,000–5,000`（近期共識 `3,000`） | `4.65–9.08` |

---

## 5. 假設條件、工程限制與未解問題

1. **商業化門檻與實場數據稀缺**：截至 2015 年，除 Ignik Sikumi 置換試驗持續約 6 週外，其餘降壓／熱激實場試驗皆未超過 `6 days`；論文指出需先完成 **`20,000–30,000 m³/d` 持續約 2 個月**的長期穩產試驗，才可能跨過商業化門檻（陸上小型商轉預估 `2025–2030`，海域顯著產量落在 `2030` 年後）。
2. **出砂與產水管理**：海相未固結砂層在降壓分解後容易出砂（Sand Production）並伴隨大量產水，直接中斷井筒穩定運行。
3. **水合物再生成（Re-formation）被理論模型忽略**：多數數值模型假設分解後不會再生成，但實場環境難以如實驗室精控，降壓途中若有自由氣存在仍可能引發局部再生成（文獻 [140] 實測 `14.5 MPa` 降壓時出現 `0.26–0.35 K` 溫升）。
4. **地質力學與環境風險**：分解造成沉積物強度喪失可能引發海床沉降或海底滑坡；$\text{CH}_4$ 的百年 GWP 約為 $\text{CO}_2$ 的 `21` 倍，但易受全球暖化觸發（Clathrate Gun 假說）的是淺層非經濟水合物，而非深層高飽和砂層儲層。

---

## 6. 知識庫關聯與觀點衝突

### 知識庫連結
- **核心概念**：[[Natural Gas Hydrates (NGH)]]、[[Self-Preservation Phenomenon]]、[[Hydrate-Bearing Sediment Geomechanics]]
- **開採與轉換方法**：[[Conventional NGH Dissociation Methods]]、[[CH4-CO2 Hydrate Exchange Process]]
- **綜合比較（重點）**：[[NGH Field Trials and Commercialization Comparison]]

### 論文內揭露之關鍵觀點衝突與條件差異

> [!warning] 觀點衝突 / 條件差異：Messoyakha 氣田是否真由水合物供氣
> - **Makogon & Omelchenko (2013)**：主張西伯利亞 Messoyakha 氣田累計 `12.9 × 10^9 m³` 產氣中，有 `5.4 × 10^9 m³` 來自降壓引發的水合物分解。
> - **Collett & Ginsburg (1998)**：指出該氣田實際產水量比水合物分解理論產水量低了**至少 3 個數量級**，因此質疑產氣是否真源於水合物層。

> [!warning] 觀點衝突 / 條件差異：實驗室與實場儲層的主控瓶頸不同
> - **實驗室尺度研究**：多數降壓實驗（如 `0.1–8.4 MPa` 小型反應釜）顯示**傳熱（Heat Transfer）**與分解動力學是產氣速率的主控因子。
> - **大尺度儲層數值模擬**：如 `TOUGH-Fx/Hydrate` 與三維多相流模擬指出，在實場尺度下水合物分解動力學影響甚微，**地層滲透率與流體流動特性（Flow Factors）**才是決定性瓶頸。
