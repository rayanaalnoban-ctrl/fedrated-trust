# ZT-TrustFed: 3-Client Federated Intrusion Detection (CIC23 + CIC17 + BOT)
[![DOI](https://zenodo.org/badge/1171576535.svg)](https://doi.org/10.5281/zenodo.18862595)
This repository provides a complete experimental pipeline for **federated intrusion detection** across heterogeneous security datasets using **Zero-Trust inspired trust aggregation**, **FedProx** for non-IID robustness, and **FedBN-style** client-specific BatchNorm statistics.

✅ Robust CSV loading (local folder)  
✅ Global feature union (CIC + BOT) → shared input space  
✅ Cleaning + clipping + per-client scaling  
✅ Strong imbalance handling (class weights + balanced sampling)  
✅ **FedProx** + **Trust-weighted aggregation**  
✅ **FedBN-style** BatchNorm (client-specific running stats)  
✅ Feature selection (Mutual Information top-k)  
✅ Cross-dataset evaluation per round (Acc / BalancedAcc / MacroF1)  
✅ Final detailed metrics (Precision/Recall/F1, ROC/PR, Confusion Matrix)  
✅ **Adversarial robustness** (FGSM)  
✅ **Ablation study** (FedAvg / FedProx / TrustOnly / FedProx+Trust)  
✅ **Privacy–utility tradeoff** via DP-like gradient noise  
✅ **HTML report export** with all tables + plots embedded  

---

## 1) Project Structure (Recommended)

```text
ZT-TrustFed-FL-IDS/
│
├─ data/                         # put CSV files here
│   ├─ CIC.csv
│   ├─ CICIDS2017.csv
│   └─ IoT_Botnet_Final_10_best_Training.csv
│
├─ src/
│   └─ new.ipynb     # your full code file
│
├─ results/
│   └─ zt_trustfed_report.html   # generated HTML report
│
├─ README.md
└─ requirements.txt
