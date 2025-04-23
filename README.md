# DSPO: Direct Score Preference Optimization for Diffusion Model Alignment

**This repository is an official PyTorch implementation of**  ["DSPO: Direct Score Preference Optimization for Diffusion Model Alignment"](https://openreview.net/pdf?id=DomBynQsqt) (ICLR 2025)

<img width="987" alt="image" src="model/model.jpg">

## Environment Preparation 
```
conda create -n DSPO python=3.10 && conda activate DSPO
```

```
pip install -r requirements.txt
```
# Model Training
## Training on Stable Diffusion v1.5
The hyperparameter $\beta$ can be searched by $\{0.001, 0.01, 0.05\}$, the best steps can be 500, 1000, 1500
```bash
bash sd15.sh
```
## Training on Stable Diffusion XL
The hyperparameter $\beta$ can be searched by $\{1000, 2000, 3000, 4000, 5000\}$, the best steps can be 600,700
```bash
bash sdxl.sh
```