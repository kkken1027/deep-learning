### Convolution 介紹
- 原理<BR>
卷積運算中的mask 稱為Convolution Kernel (卷積核) 其數量可調整，由不同的卷積核權重組合，就可以偵測出邊、角、去噪音及銳化的效果，也克服了回歸常受到異常點而導致錯誤結果的缺點，相對於隱藏層(Dense)連接所有的神經元，卷積層則是局部連接(連接感知域)，故比起Dense不需要很大的記憶體與運算時間。

##### 由以下圖做釋義
![avatar](https://cdn-images-1.medium.com/max/800/0*qhfRwuiidfqdIV4v.jpg)
![avatar](./img/conv2.gif)

##### Reference
- [1] https://engineering.huew.co/introduction-to-convolution-neural-networks-18981d1cd09a
- [2] https://ithelp.ithome.com.tw/articles/10191820
