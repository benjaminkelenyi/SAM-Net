# SAM-Net Implementation
![image](https://github.com/benjaminkelenyi/SAM-Net/assets/22835687/4b787ddd-6111-478d-97b3-76c6088f5d85)

This is a PyTorch implementation of SAM-Net paper and can be used to reproduce the results in the paper.

This work focuses on detector-free image matching. 

This repo contains training, evaluation and basic demo scripts used in our paper.

A large part of the code base is borrowed from the [LoFTR Repository](https://github.com/zju3dv/LoFTR) under its own separate license, terms and conditions.

## Installation 
```bash
conda env create -f environment.yaml
conda activate samnet
```

## Get started
A demo to match one image pair is provided. To get a quick start, 

```bash
cd demo
python demo.py
```


## Data Preparation
Please follow the [training doc](docs/TRAINING.md) for data organization



## Evaluation


### 1. ScanNet Evaluation 
```bash
cd scripts/reproduce_test
bash indoor.sh
```

### 2. MegaDepth Evaluation
 ```bash
cd scripts/reproduce_test
bash outdoor.sh
```



## Training

### 1. ScanNet Training
```bash
cd scripts/reproduce_train
bash indoor.sh
```

### 2. MegaDepth Training
```bash
cd scripts/reproduce_train
bash outdoor.sh
```

## Useful data:
The extra files that you need to run SAM-Net can be found [here](https://drive.google.com/drive/folders/1SyWAScRUpcC32LSTZcku16ZHMfMctymR?usp=drive_link).
* dump
* data
* pixloc
* assets


