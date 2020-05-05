# Fraud Detection with Deep Learning

Click and run code by launching Binder 
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jimmyhu4/fraud-detection/master)

## Running Environment

The main packages you need to install

```
1. python 2.7 
2. tensorflow 1.5.0
```

## DateSet
For experiments, we evaluate **SAFE** on two real-world datasets: twitter and wiki which have been attached in [twitter/](https://github.com/PanpanZheng/SAFE/tree/master/twitter) and [wiki/](https://github.com/PanpanZheng/SAFE/tree/master/wiki), respectively.


## Model Evaluation

The command lines for SAFE and baselines go as follow

* **SAFE** 
```
    python framework/safe.py $1
```

* **M-LSTM** 

```
    python framework/base_rnn.py $1
```

* **CPH & SVM** 

```
    python framework/safe_baselines.py $1
```

**where** *$1* refers to datasets on which the model runs, and it can be assigned as 'twitter' or 'wiki'.


* **Weibull & other distributions**
```
    python framework/safe_distr.py $1 $2
```

**where** *$1* refers to the corresponding distributions and it can be assigned as 'exp' (exponential), 'ray' (Rayleigh) and 'poi' (poisson); *$2* denotes the datasets, 'twitter' or 'wiki'.



## Citation

SAFE: A Neural Survival Analysis Model for Fraud Early Detection: Arxiv https://arxiv.org/abs/1809.04683v1