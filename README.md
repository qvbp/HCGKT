# HCGKT(IJCAI 2025)

## Installation
Use the following command to install HCGKT:

Create conda envirment.

```
conda create --name=hcgkt python=3.8.17
source activate hcgkt
```


```
cd HCGKT
pip install -e .

```

## Datasets Download & Preprocess

### Download
you can download the datasets we used from [algebra2005](https://pslcdatashop.web.cmu.edu/KDDCup/) [bridge2006](https://pslcdatashop.web.cmu.edu/KDDCup/) [peiyou](https://drive.google.com/file/d/1eFiIYyh5O2V90RA0brammGH6EpHvPDQe/view)

### Preprocess
```
cd examples
python data_preprocess.py --dataset_name=algebra2005
```

## HCGKT Train & Evaluate

### Train
```
python wandb_hcgkt_train.py  --dataset_name=algebra2005
```

### Evaluate
```
python wandb_predict.py  --save_dir="/path-of-previous-trained-model"
```

## Hyper-parameter
See examples/seedwandb/hcgkt.yaml
