## Part Grouping Network (PGN)
Authors: Ke Gong, Xiaodan Liang, Yicheng Li, Yimin Chen, Ming Yang and Liang Lin

Paper: "Instance-level Human Parsing via Part Grouping Network", ECCV 2018 (Oral). [PDN] (https://arxiv.org/pdf/1202.00157.pdf)

[Github repo]: https://github.com/Engineering-Course/CIHP_PGN


### Inference - Run test or valuation 
1. Pre-trained model on CIHP and Pascal-Person-Part are saved in checkpoint folder in corresponding names.
2. Prepare the images and store in $HOME/datasets.
3. Run test_pgn.py for testing CIHP and test_pascal for testing Pascal pre-trained model.
4. The results are saved in $HOME/output with corresponding names

### Training
1. Download the pre-trained model and store in $HOME/checkpoint.
2. Download CIHP dataset, Pascal dataset and save in $HOME/datasets
3. For CIHP dataset, you need to generate the edge labels and left-right flipping labels (optional). We have provided a script for reference.
4. Run train_pgn.py to train PGN.
5. Use test_pgn.py to generate the results with the trained models.
6. The instance tool is used for instance partition process from semantic part segmentation maps and instance-aware edge maps, which is written in MATLAB.

## Related work
+ Self-supervised Structure-sensitive Learning [SSL](https://github.com/Engineering-Course/LIP_SSL), CVPR2017
+ Joint Body Parsing & Pose Estimation Network  [JPPNet](https://github.com/Engineering-Course/LIP_JPPNet), T-PAMI2018
+ Graphonomy: Universal Human Parsing via Graph Transfer Learning [Graphonomy](https://github.com/Gaoyiminggithub/Graphonomy), CVPR2019

## System recommendation
+ Scripts run in python 2.7, Ubuntu 18.04, cuda 10.0, cuDNN 7.4, GPU  GeForce GTX 1080 8G caused no errors but minor warnings 
+ Data preparation scripts run on Matlab (2018Rb) 
+ Site packages required listed in requirements.txt

## Data pre-process for trainning:
Visit issue section on original github repo

