### Pooling 介紹
- 原理<BR>
通常接於 Convolution layer之後，有效的縮小圖片的尺寸(降維)，減少最後全連接層的參數(減參)，加快計算速度，減少過擬合，並保持輸入矩陣的平移不變性，與卷積層類似，通過一個濾波器結構完成，不同的是濾波器計算的不是加權求和，而是區域內最大值或平均值兩種。

* 最大值 ( max pooling )<BR>
提取紋理效果好，如同做了特徵選擇，提供非線性。缺點，失去特徵位址與強度訊息，因為空間中只提取最大值，即使特徵出現多次。
* 平均值 ( average pooling )<BR>
保留更多圖像背景，常接於DenseNet 之間，降維同時也保留特徵訊息。缺點，卷積層參數誤差造成pooling 後估計值偏移。

##### 由以下圖做釋義
![avatar](https://www.researchgate.net/profile/Hanli_Wang2/publication/300020038/figure/fig2/AS:404961465782275@1473561745471/Toy-example-illustrating-the-drawbacks-of-max-pooling-and-average-pooling.png)
![avatar](http://ufldl.stanford.edu/wiki/images/0/08/Pooling_schematic.gif)

##### Reference
- http://ufldl.stanford.edu/wiki/index.php/Pooling
- https://www.researchgate.net/figure/Toy-example-illustrating-the-drawbacks-of-max-pooling-and-average-pooling_fig2_300020038
- https://www.slideshare.net/matsukenbook/deep-learning-chap6-convolutional-neural-net
