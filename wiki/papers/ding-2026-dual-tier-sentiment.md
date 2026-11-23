# The Dual-Tier Sentiment Framework: Scalable Multimodal UX Attribution in Web Search

- 作者：Yi Ding、Gaurav Kumar、Rui Min、Isabella Ye、Bhavika Goyal、Emilio Antunez、Huihui Chen、Ke Xu、Xiaowei Sun、Xin Xu、Huijie Feng、Pradyumna Narayana、Golnaz Farhadi
- 年份與版本：2026，arXiv 預印本 v1（2611.27899）
- 原始資料：[arXiv v1](https://arxiv.org/abs/2611.27899v1)，本機 `raw/2611.27899v1.pdf`

## 研究問題與方法

作者針對搜尋 A/B 實驗設計兩層評估。第一層（Macro System）用微調的 Gemini XS 與遙測特徵偵測整體滿意度退化。第二層（Micro System）用 Gemini 3.0 Pro 評估渲染後的搜尋結果頁與各區塊位置，以 User Toil 估計使用者達到滿意結果所需的努力，並以提示最佳化和模型評審輔助診斷。（PDF 第 1–5 頁，摘要、圖 1–2）

兩層**並行評估**。從使用者體驗的角度，兩個上線條件必須同時成立：整頁體驗未退化，且局部 User Toil 有改善。（PDF 第 2 頁，圖 1）

## 作者報告的結果

- 在超過 50 萬筆保留資料上，第一層的 PR-AUC 提升 9.8%。在 12 個保留實驗中，摘要報告維持已驗證退化的召回表現，精確率相對提升約 20%。（PDF 第 1 頁，摘要）
- 第二層的 F1 改善超過 6.5%。這個指標屬於局部診斷系統，與第一層的 PR-AUC 衡量不同任務。（PDF 第 1 頁，摘要）

## 限制與文獻回顧用途

多模態渲染和推論成本使第二層採非同步批次評估（PDF 第 7 頁，Limitations）。文獻回顧可引用此案例比較整體篩查與局部診斷如何搭配，並把遙測代理指標、調查和模型評審分別記錄。
