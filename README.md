# AutoGraph

This repo is no longer maintained. Please refer to [https://github.com/AutoML-Research/AutoGraph-KDDCup2020](https://github.com/AutoML-Research/AutoGraph-KDDCup2020)

## Introduction
This is the official repo for hosting AutoGraph challenge datasets/code from KDD Cup 2020, targeting automated node classification task. To that end, we provide in this repo 13 datasets from public and private sources to fully evaluate the generalization ability of AutoML algorithms.

Update (2021/08/23):

- sample data under starting kit added
- release all available datasets with licenses from AutoGraph chellenge (data_autograph.zip)

Update (2021/08/10):

- starting kit code added
- winning solutions added

## Running locally

We provide full details for evaluating locally. Please download the datasets and put under the folder `src/data`. Then pull the prepared docker `nehzux/kddcup2020:v2` and run command
`docker run --gpus=0 -it --rm -v "$(pwd):/app/autograph" -w /app/autograph nehzux/kddcup2020:v2`

Go to the directory of `run_local_test.py` and run `python run_local_test.py --dataset_dir=data/a --code_dir=code_submission/0_baseline` for testing baseline on dataset a.

## Dataset license:

We include 13 datasets in total here in this repository. 10 datasets come from public datasets and 3 come from 4paradigm. We conclude the licenses for each dataset below. If you find anything inappropriate and have any question regrading the license, please contact us by: xuzhen[AT]4paradigm[DOT]com


| Dataset ID  | Origin Source | License |
| ------------- | ------------- | ------------- |
| a  | Cora  | MIT  |
| b  | CiteSeer  | CC BY-NC-SA 3.0  |
| c  | Reddit  | MIT  |
| d  | 20 Newsgroups  | Credit to Ken Lang and Tom Mitchell  |
| f  | Amazon Computer  | MIT  |
| g  | Coauthor Physics  | MIT  |
| h  | ohsumed  | CC BY-NC 4.0  |
| j  | 4paradigm  | CC BY-NC 4.0  |
| k  | Amazon Photo  | MIT  |
| l  | Coauthor CS  | MIT  |
| m  | R8  | Copyright to Reuters Ltd  |
| n  | 4paradigm  | CC BY-NC 4.0  |
| o  | 4paradigm  | CC BY-NC 4.0  |



# References:
- https://github.com/aister2020/KDDCUP_2020_AutoGraph_1st_Place
- https://github.com/Unkrible/AutoGraph2020
- https://github.com/white-bird/kdd2020_GCN
