# MDR1-M4-HYB-v1: Graph neural network ensemble for P-gp substrate prediction

This repository provides the code and notebooks used to develop the MDR1-M4-HYB-v1
graph neural network (GNN) ensemble for predicting P-glycoprotein (P-gp/ABCB1/MDR1)
substrates from chemical structure.

The implementation accompanies the manuscript:

> Enokiya T., Yamaguchi T. *Graph neural network–based prediction of P-gp substrates using public bioassay and KEGG data* (submitted).

Please cite the manuscript if you use this code in academic work.

---

## Repository structure

```text
mdr1-m4-hyb-v1/
├─ README.md
├─ LICENSE
├─ env/
│   └─ requirements.txt           # Python package requirements
├─ notebooks/
│   └─ MDR1_M4_HYB_v1_training.ipynb  # End-to-end training / evaluation notebook
├─ src/
│   ├─ data_preparation.py        # Build training / external sets from raw data
│   ├─ train_mdr1_m4_hyb_v1.py    # Train cross-validated GNN ensemble
│   └─ eval_external.py           # Evaluate on external clinical-like set
└─ data/
    ├─ raw/                       # Raw public data (not included by default)
    └─ processed/                 # Preprocessed datasets used by the model
