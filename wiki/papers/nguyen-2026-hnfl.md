# Learning in Symbiosis: Heterogeneous Federated Learning with ANNs and SNNs

- 作者：Manh V. Nguyen、Liang Zhao、Bobin Deng、Xinyue Zhang、Shaoen Wu
- 年份與版本：2026，arXiv 預印本 v1（2611.27686）
- 原始資料：[arXiv v1](https://arxiv.org/abs/2611.27686v1)，本機 `raw/2611.27686v1.pdf`

## 研究問題與方法

混合神經形態聯邦學習（HNFL）讓傳統人工神經網路（ANN）與脈衝神經網路（SNN）客戶端共同訓練，同時區分可共享的參數與模型專用參數。作者用 CIFAR-10 測試 VGG9 和 ResNet 系列架構，以及重複輸入與 Poisson 編碼。（PDF 第 2–4 頁）

## 作者報告的結果

- ANN 單獨訓練的 ResNet 在 Poisson 輸入設定下，加入 SNN 客戶端後準確率由 56.60% 升至 73.45%，增加 16.85 個百分點。反向混合的另一設定中，SNN 準確率由 70.44% 升至 78.46%，增加 8.02 個百分點。兩者是特定設定的差值。（PDF 第 4 頁）
- 作者在摘要報告 SResNet 和 SVGG9 的脈衝活動分別下降 12.4% 和 22.4%。摘要把準確率增幅寫成平均改善，正文及結論的表述有差異，引用時宜使用第 4 頁的基準與設定。（PDF 第 1、4、6 頁）

## 限制與文獻回顧用途

作者指出仍需在異質的非獨立同分布（non-IID）資料上驗證泛化（PDF 第 6 頁，結論）。回顧邊緣裝置聯邦學習時，可將分類準確率、通訊輪數、脈衝活動與實機能耗列為不同評估項目。
