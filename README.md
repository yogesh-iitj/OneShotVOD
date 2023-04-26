## Requirements
* Use **python >= 3.8.5**. Conda recommended : [https://docs.anaconda.com/anaconda/install/linux/](https://docs.anaconda.com/anaconda/install/linux/)

* Use **pytorch 1.7.0 CUDA 10.2 or higher**

* Other requirements from 'requirements.txt'

**To setup environment**
```
  # create new env fsrr
  $ conda create -n qdetr

  # activate qdetr
  $ conda activate qdetr

  # install pytorch, torchvision
  $ conda install -c pytorch pytorch torchvision
  $ conda install cython scipy

  # install other dependencies
  $ pip install -r requirements.txt
```

## Pre-training
```
# Pre-train qdetr on image dataset
# set config_pre.py 
$ export CUDA_VISIBLE_DEVICES=0,1
$ python train_pre.py
```
## Training qdetr
```
# set config.py
$ export CUDA_VISIBLE_DEVICES=0,1
$ python train_pre.py
```
