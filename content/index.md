---
title: Energy & Power LLM Wiki
---

# Energy & Power LLM Wiki

這是一個以 **Karpathy LLM Wiki 模式**建置的能源工程與電力技術知識庫。原始論文由人與 LLM Agent 逐篇共讀，並以「增量編譯」的方式整理成互相連結的筆記。目前收錄 5 篇關鍵綜述論文，主題涵蓋：

- **電能儲存（EES）**：六大類儲能技術、電力系統時間尺度配對與季節性儲能缺口
- **氫能產製與儲存**：水電解（AEL / PEM / SOEC）、純度標準、金屬氫化物固態儲氫
- **電轉氣（Power-to-Gas）**：電解 → 甲烷化全鏈效率與 SNG 經濟性
- **天然氣水合物（NGH）**：晶體結構、開採方法、$\text{CH}_4$–$\text{CO}_2$ 置換與全球現場試驗

> [!info] 教學 HTML 簡報
> **<a href="./static/energy-transition-storage-hydrogen-ptg-ngh.html" data-router-ignore target="_blank" rel="noopener">能源轉型全鏈條工程解析：儲電、氫能、電轉氣與天然氣水合物 ↗</a>**
>
> 共 12 頁，可用鍵盤翻頁（← / → / Space），按 `T` 開關目錄、按 `F` 進入全螢幕；內含 KaTeX 方程式、Chart.js 數據圖與 SVG 架構圖。

---

## 四層知識結構

| 層級 | 資料夾 | 內容 |
| --- | --- | --- |
| **Sources** | `sources/` | 單篇論文精讀：研究問題、方法、關鍵數據與限制 |
| **Concepts** | `concepts/` | 核心概念、物理定義與評估指標 |
| **Methods** | `methods/` | 技術路線、製程、拓撲與方法比較 |
| **Synthesis** | `synthesis/` | 跨論文整合比較、觀點衝突與商業化評估 |

閱讀順序建議：先從下方兩個 **Synthesis 樞紐頁**掌握全貌，再沿著 `[[Wikilinks]]` 深入個別概念與方法，最後回到 Sources 查核原文數據。右側的**關係圖（Graph View）**顯示所有筆記之間的連結。

---

## Synthesis 樞紐頁

- [[Integrated Energy Storage, Hydrogen, PtG and NGH Commercialization Comparison]]：整合全部 5 篇論文，跨技術比較儲電、氫能、電轉氣與 NGH 的效率、實場試驗與商業化經濟性。
- [[NGH Field Trials and Commercialization Comparison]]：天然氣水合物全球五大現場試驗、成本與商業化門檻、環境風險治理。

---

## Sources（單篇論文精讀）

- [[Overview of Electrical Energy Storage Technologies (2015)]]
- [[Review of Natural Gas Hydrates as an Energy Resource (2016)]]
- [[Renewable Power-to-Gas Review (2016)]]
- [[Hydrogen Energy Economy and Storage Review (2019)]]
- [[Hydrogen Production for Energy Overview (2020)]]

## Concepts

- [[Electrical Energy Storage (EES) Classification]]
- [[Hydrogen Cleanness Index and Purity Standards]]
- [[Natural Gas Hydrates (NGH)]]
- [[Self-Preservation Phenomenon]]
- [[Hydrate-Bearing Sediment Geomechanics]]

## Methods

- [[Water Electrolysis Technologies (AEL, PEM, SOEC)]]
- [[Hydrogen Storage Technologies and Metal Hydrides]]
- [[Power-to-Gas and Methanation Processes]]
- [[Conventional NGH Dissociation Methods]]
- [[CH4-CO2 Hydrate Exchange Process]]

---

建置與維護紀錄請見 [[log|知識庫操作日誌]]。本站只發布整理後的筆記與簡報，**不包含原始論文 PDF**。
