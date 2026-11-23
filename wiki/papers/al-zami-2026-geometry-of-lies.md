# The Geometry of Lies: Knowledge and Persona Directions for Detecting Deception in Large Language Models

- 作者：Md. Abdullah Al Zami、Suraiya Shanaz、Mahdi Hasan、Shoaib Ahmed Dipu、Farig Yousuf Sadeque、Md. Sabbir Ahmed
- 年份與版本：2026，arXiv 預印本 v1（2611.26545）
- 原始資料：[arXiv v1](https://arxiv.org/abs/2611.26545v1)，本機 `raw/2611.26545v1.pdf`

## 研究問題與方法

當模型用同一句「我不知道」表達誠實否認或否認已知答案時，能否用模型內部活化辨別兩者？作者比較**角色方向**（persona direction）和**知識方向**（knowledge direction）。前者取誠實與欺騙角色扮演的平均活化差異。後者比較有已知答案的問題與刻意不可回答的問題，兩組問題都接上同一句事先寫好的否認。研究以 Liars’ Bench 與四個模型評估。（PDF 第 4–5 頁，§3）

## 作者報告的結果

- 在相同回答文字的 HP-KR 子集中，Llama 和 Mistral 的知識方向 AUROC 分別為 0.793 與 0.840，超過各自的隨機方向上界。Qwen 只小幅超過，Gemma 未超過。在這項控制下，多數角色方向未明顯超過隨機方向範圍或其邊界。（PDF 第 7、9 頁，§4.3、表 1）
- Llama 的同層監督式探針在 HP-KR 的 AUROC 為 0.936，但按基準設定的門檻，139 個欺騙案例中沒有標出任何一個。（PDF 第 6 頁，§4.1）

## 限制與文獻回顧用途

兩組回答文字相同，但對應的問題不同，結果仍可能反映題目差異。作者先看到 HP-KR 的失敗才設計新角色與知識方向，HP-KR 因此屬於方法開發資料（PDF 第 11–12 頁，§7）。對文獻回顧的啟示是同時記錄排序指標、固定門檻的實際檢出率，以及評估時控制了哪些輸入特徵。
