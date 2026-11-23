# SLICR: Strategy Logic-Guided Multi-Agent Reinforcement Learning

- 作者：Arshia Rafieioskouie、Matthew Lucas、Tzu-Han Hsu、Borzoo Bonakdarpour
- 年份與版本：2026，arXiv 預印本 v1（2611.27865）
- 原始資料：[arXiv v1 PDF](https://arxiv.org/pdf/2611.27865v1)，本機 `raw/2611.27865v1.pdf`

## 研究問題與方法

SLICR 用策略邏輯（Strategy Logic, SL）量化代理的策略，以線性時序邏輯（LTL）描述目標和約束。方法在部分可觀測隨機博弈中，從行動和觀察歷程表示策略情境，再據此學習回應。訓練時加入規範的穩健度訊號，並以屏蔽機制排除作者定義的不合理策略所對應的經驗。（PDF 第 2–8 頁，§3–5、圖 2）

## 作者報告的結果

- 在 Predator–Prey、Google Research Football 和擴充版 SMAC-HARD 上測試。足球 R2S 情境相對 LIAM，對已見與未見策略每 100 場最多分別多進約 30 與 20 球。（PDF 第 9 頁，圖 3a）
- 在 IPPO 的 SMAC-HARD 3s_vs_3z 未見策略條件，作者報告 SLICR 勝率約 80%，LIAM 約 10%。這是特定地圖及訓練設定的結果。（PDF 第 10 頁，圖 3i）

## 限制與文獻回顧用途

理論結果以情境表示能保存資訊、回應函數具有足夠表達能力等條件為前提（定理 5.3）。比較規範引導研究時，可用本篇區分「對手策略泛化」與「更換任務目標後的泛化」，並分別記錄已見與未見對手的結果。
