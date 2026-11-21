---
type: method
category: "extraction"
tags:
  - method
  - natural-gas-hydrates
  - depressurization
  - thermal-stimulation
  - chemical-inhibitor
aliases:
  - "傳統水合物分解開採法"
  - "熱激法與降壓法"
sources_count: 1
updated: 2026-11-21
---

# Conventional NGH Dissociation Methods

與常規氣田或頁岩氣不同，開採 [[Natural Gas Hydrates (NGH)|天然氣水合物]] 必須先打破其溫壓相平衡以進行**原位分解（In Situ Dissociation）**。以典型海床沉積物工況（`4 °C, 8 MPa`）為例，觸發分解至少需滿足以下條件之一：升溫 $\Delta T \ge 7\ \text{K}$、降壓 $\Delta P \ge 4.2\ \text{MPa}$，或注入約 `30 wt.%` 的乙二醇（EG）[[Review of Natural Gas Hydrates as an Energy Resource (2016)]]。

---

## 1. 三大單一分解法比較

| 方法 | 核心原理 | 優勢 | 核心工程瓶頸與限制 |
| --- | --- | --- | --- |
| **熱激法（Thermal Stimulation）** | 外部供熱（熱水／蒸汽注入、電磁微波、原位燃燒）使局部溫度高於相平衡曲線 | 分解驅動力直觀、高熱通量（`255–13,700 W/m²`）可避開 [[Self-Preservation Phenomenon|自我保護效應]] | 熱流體沿井筒長距離輸送熱損極大；能效低（高水合物飽和度、低注水率與低溫雖可提高能效，卻導致產氣過慢） |
| **降壓法（Depressurization）** | 降低井底壓力至當地溫度對應之相平衡壓力以下 | **能效最高**、最貼近常規油氣技術、為目前實場主力（Mallik、Nankai Trough） | 單純降壓產氣速率偏低；吸熱分解易造成近井溫度緩衝／結冰（`< 272.7 K`）；需在低井壓（快產）與高井壓（保地層穩定）間取捨 |
| **化學抑制劑注入（Chemical Inhibitor Injection）** | 注入熱力學抑制劑（甲醇、乙二醇 EG、NaCl 鹽水）使相平衡曲線移向高壓低溫 | 分解可同時發生於整個樣品（非僅限出口端）；降低分解熱，使熱效率提升約 `3.5` 倍 | 實驗室所需「抑制劑／水合物」比例極高，實場大規模注入不具經濟性與輸送可行性 |

---

## 2. 各方法之關鍵實驗洞察與條件差異

### 2.1 熱激法替代傳熱方案
- **電磁／微波加熱（Electromagnetic / Microwave Heating）**：將熱源直接置於井底，避免熱水沿井管傳遞的熱損失；模擬與實驗室微波測試均證實可顯著提升能效與分解速率。
- **原位燃燒（In Situ Combustion）**：燃燒部分原位甲烷供熱，並具備耦合 $\text{CO}_2$ 封存潛力。

> [!warning] 觀點衝突 / 條件差異：原位燃燒能效的模擬與實驗落差
> - **Castaldi et al. (2007) 早期模擬**：預測原位燃燒能源效率可高達 `90%`。
> - **Fitzgerald et al. (2012) 實驗室實測**：實際能效顯著低於早期模擬預測，且實場必須嚴格驗證製程安全（避免失控燃燒導致大量甲烷洩漏）。

### 2.2 降壓法的尺度瓶頸與再生成風險
- **三階段產氣特徵**（南海神狐模擬工況：`5.8 L` 反應釜、`281.15 K`、初始 `11.8 MPa` 降壓至 `4.5–5.6 MPa`）：依序經歷**自由氣產出 → 混合氣產出 → 水合物氣產出**，且流阻隨分解進行而下降。
- **井底壓力權衡**（二維模擬，`4.5 °C, 4.0 MPa`，平衡壓 `3.875 MPa`）：井壓降至 `1.0`、`2.0`、`3.0 MPa` 時，越低壓產氣越快，但較高井壓有助維持 [[Hydrate-Bearing Sediment Geomechanics|儲層地質力學穩定]]。
- **低滲透率瓶頸**：祁連山永凍土單直井降壓模擬顯示，在低滲透率儲層中總採收率僅 `2.3%`。
- **水合物再生成**：多數理論模型假設分解後不再生，但實測於 `14.5 MPa` 降壓時曾觀測到 `0.26–0.35 K` 溫升，證實自由氣存在時可能發生局部再生成。

> [!warning] 觀點衝突 / 條件差異：降壓法的主控機制（實驗室 vs. 實場）
> - **實驗室尺度**：快速降壓至 `0.1 MPa`（`272–289 K`）或 `0.2–8.4 MPa`（`285–286 K`）時，<strong>傳熱速率（Heat Flow）</strong>是主控因子。
> - **實場大儲層模擬**：`TOUGH-Fx/Hydrate`（擬合 $k_d \sim 10^4\ \text{mol}\cdot\text{m}^{-2}\cdot\text{Pa}^{-1}\cdot\text{s}^{-1}$）與三維多相流模擬皆指出，實場產氣主要受制於**滲透率、自由氣比例與多相流動特性**，而非本徵分解動力學。

### 2.3 化學抑制劑：EG 與 NaCl 濃度的不同行為
- **乙二醇（EG）**：因市場可得性高、毒性低於甲醇、密度大而表現較佳；提高 EG 濃度可使氣體產出率單調上升，且存在對應「井口下方孔隙體積」的最佳注入效率點。
- **鹽水（NaCl）**：低濃度（`3.45 wt.%`）可有效促進分解並提升產氣；但過高濃度（`20 wt.%`）反而因砂岩孔隙內析出不透水 NaCl 鹽層、堵塞孔道降低滲透率而抑制分解（此外 NaCl 在動力學上亦具抑制作用）。

---

## 3. 複合開採法（Combination Approaches）

為彌補單一方法「降壓太慢、熱激太耗能」的缺陷，研究普遍指向複合開採 [[Review of Natural Gas Hydrates as an Energy Resource (2016)]]：
1. **吞吐法（Huff-and-Puff）**：單直井循環執行「注熱水（`160 °C, 0.2 L/min`, `10–30 min`）→ 燜井（`30 min`）→ 降壓產氣（`10 min`）」。在 `117.8 L` 中試反應釜（PHS，起始 `4.7 MPa`）中達成高氣水比 $R_{\text{GW}} > 55\ \text{m}^3\ \text{CH}_4\text{ (STP)}/\text{m}^3\ \text{water}$，但燜井期壓力回升會削弱分解驅動力。
2. **加熱井筒 + 降壓**：於 Toyoura 砂（`40%` 水合物飽和度、`6 MPa` 井壓）下，`90 min` 內平均產氣量較單純降壓提高 **`3.6` 倍**。
3. **多井複合系統（Five-Spot / SAGD / SAAD）**：
   - **五點法（Five-Spot）熱激 + 降壓**：生產時間最短，能效為單純五點熱激法的 **`15` 倍**（降壓降低局部溫度進而強化熱傳）；倒五點注水法（Inverted Five-Spot）能效比吞吐法再提升約 **`33%`**。
   - **雙水平井 SAGD / SAAD**（`117.8 L` 壓力釜，結合熱激、降壓與熱鹽水注入）：反重力排洩法（SAAD，生產井位於注入井上方）較重力輔助法（SAGD）產氣更多、產水更少且長期能效更高。

---

## 4. 相關知識庫連結
- 來源文獻：[[Review of Natural Gas Hydrates as an Energy Resource (2016)]]
- 相關概念：[[Natural Gas Hydrates (NGH)]]、[[Self-Preservation Phenomenon]]、[[Hydrate-Bearing Sediment Geomechanics]]
- 替代路線：[[CH4-CO2 Hydrate Exchange Process]]
- 實場驗證：[[NGH Field Trials and Commercialization Comparison]]
