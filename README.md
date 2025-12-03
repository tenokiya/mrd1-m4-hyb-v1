# MDR1-M4-HYB-v1: Graph neural network ensemble for P-gp substrate prediction

This repository provides the code and notebook used to develop the MDR1-M4-HYB-v1
graph neural network (GNN) ensemble for predicting P-glycoprotein (P-gp/ABCB1/MDR1)
substrates from chemical structure.

The implementation accompanies the manuscript:

> Enokiya T., Yamaguchi T.
> Graph neural network–based prediction of P-gp substrates using public bioassay and KEGG data.
> (submitted to ADMET and DMPK)

## Contents

- `MDR_ver7.ipynb`: end-to-end notebook for data preparation, model training and evaluation.

## Data sources

We use only public data:

- PubChem BioAssays AID 1346986 and 1346987 (KB-3-1 / KB-8-5-11 cells)
- KEGG BRITE MDR1 substrate annotations and FDA label information

Raw data are not redistributed here. The notebook shows how to reconstruct
the training and external evaluation sets from these public sources.

## License

See the `LICENSE` file for details.
