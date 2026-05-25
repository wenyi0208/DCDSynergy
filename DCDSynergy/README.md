# DCDSynergy: A Drug–Cell Feature Fusion Framework for Predicting Synergistic Drug Combinations with Deep Learning

This code repository is the supporting material in the paper. In this paper, we propose a novel approach called DCDSynergy, which leverages the integration of chemical structure data and gene expression data to predict the synergistic effects of drug combinations.
<img width="2906" height="1022" alt="DCDSynergy" src="https://github.com/user-attachments/assets/f88c1acc-3c98-4268-bcc9-ed609041b08b" />


## Requirements

The third-party dependencies required for model running are listed in [environment.yaml](./environment.yml). You can install the environment by running

```bash
conda env create -f environment.yml
```

## Data preparation

All data used in this paper are public and accessible. The relevant dataset has been stored in [Cloud Drive](https://drive.google.com/drive/folders/1mgCB3NJJB4RXE_KrxmdlQK7_LXtU66kh?usp=sharing) and can be downloaded to the `./data/raw/` folder. Please refer to the [DATA README](./data/raw/README.md) for the source of each file.

After downloading the relevant dataset and place it in the `./data/raw/` folder you can generate the training set and test set by running

```bash
python dataproc.py
```

## Training

After generating the traning set and test set `(ONEIL_train.pkl、ONEIL_test.pkl)` you can start training the model by running

```bash
python main.py
```
