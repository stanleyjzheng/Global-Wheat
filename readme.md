# About Global Wheat

Global wheat was my first Kaggle competition and the first Kaggle competition I have worked full-time on. I joined about 2 weeks before the end, while other participants had 2 months. 

This folder contains training and inference jupyter notebooks from my team, AaZz, during Global Wheat. I worked primarily on You Only Look Once v4, while my teammate worked on EfficientDet.

The original intention was to ensemble, but we ran out of time. With over 6000 combined lines of code and tens of models from each of us, it is quite the task to ensemble. However, this is still my primary goal and a work in progress (albeit to late submissions). Note that the EfficientDet folder does not have a readme, but see the YOLOv4's readme (the filenames and functions are similar).

We also did not have time to implement replicable cross-validation on our training pipelines. As a result, it was difficult to compare our models on anything other than the public leaderboard. We ended up overfitting slightly, falling from 44th to 74th. If we had chosen [Version 19](https://www.kaggle.com/stanleyjzheng/yolov4pl-oof?scriptVersionId=40172709) of my YOLOv4 inference, we would have achieved 39th place. Nonetheless, I am very proud of my achievement for my first competition. I put a ton of time in over 2 weeks, so I am very pleased with this performance. 

In the coming weeks, expect to see performance metrics alongside source code to ensemble YOLOv4 alongside Effdet.

## Performance (sorted by Private Leaderboard)
|Model|Public Leaderboard|Private Leaderboard|Pseudolabels|Final Submission
|:-----:|:-----:|:-----:|:---:|:---:|
|YOLOv4|0.7406|0.6625|Y|N|
|Effdet D6|0.7594|0.6557|Y|Y|
|Effdet D7|0.7522|0.6469|Y|Y|
|YOLOv4|0.7115|0.6371|N|N|
|Effdet D6|0.7044|0.6182|N|N|
|Effdet D7|0.6921|0.6093|N|N|

Ensemble will be added soon (YOLOv4 pseudolabelling for Effdet, Effdet pseudolabelling for YOLOv4, WBF pseudolabels and final trained model, WBF without pseudolabels)