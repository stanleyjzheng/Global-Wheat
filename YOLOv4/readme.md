# You Only Look Once v4 (YOLOv4)

The training pipeline is detailed in `train.ipynb`. To create the dataset, run `labeltoYOLO.ipynb` after modifying the file paths to `train.csv` downloaded from [Global Wheat](https://www.kaggle.com/c/global-wheat-detection/data). 

There are two possible inference files. Firstly, `WBFinference.ipynb` uses Weighted Boxes Fusion (WBF) to ensemble over test time augmentation (TTA). This is a baseline inference.

Next, `Pseudoinference.ipynb` uses self-train pseudolabelling to finetune the model on the test data.

Using the baseline inference combined with the model created with `train.cfg`, a public score of 0.7115 and a private score of 0.6371 is attained. With bayesian optimization and self-training pseudolabels, a private score of 0.6498 and a public score of 0.7432 is attained. 