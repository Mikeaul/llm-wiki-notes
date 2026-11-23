# MetaRigor: From Agentic Automation to Verifiable End-to-End Meta-Analysis Through Scientific Decision Boundaries

- 作者：Yifeng Xie、Chenke Li、Yangshuo Miao、Jingyuan Zheng、Mingxuan Liu、Feiwei Qin、Yaqi Wang、Huiyu Zhou、Yifei Chen
- 年份與版本：2026，arXiv 預印本 v1（2611.27713）
- 原始資料：[arXiv v1](https://arxiv.org/abs/2611.27713v1)，本機 `raw/2611.27713v1.pdf`

## 研究問題與方法

MetaRigor 把結果記為「研究 × 目標」（Study × Target），保留比較組、族群、結局、時間點及分析條件。任務契約（Task Contracts）界定可用事實和決策，模型處理依賴上下文的語意判讀，程式負責可形式化的計算、驗證與來源綁定。流程涵蓋證據取得、資料擷取、偏誤風險、證據確定性和稿件生成。（PDF 第 5–8 頁）

## 作者報告的結果

- 在分階段比較中，完整資料擷取的 F1 為 86.29%，證據確定性的領域層級判斷一致率為 80.20%。（PDF 第 9 頁，表 2）
- 七案例的下游端到端比較中，整體 F1 為 77.01%，最高比較基準為 67.23%，相差 9.78 個百分點。這個比較涵蓋資料擷取至稿件生成。（PDF 第 24–25 頁，附錄 G、表 20）
- 檔案追蹤顯示，結局或時間點配錯可能改變統計輸入及偏誤評估對象，並一路傳到報告。（PDF 第 26 頁，附錄 G.3）

## 限制與文獻回顧用途

端到端比較只有七個案例，作者指出仍需更廣泛驗證（PDF 第 11、24 頁）。對本 Wiki 的啟示是保留結果的原文位置及適用條件，尤其同篇論文報告多個時間點或比較組時。這是 Wiki 的整理推論。
