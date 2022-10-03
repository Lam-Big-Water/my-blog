---
title: 页面抖动
---
# 时有时无的滚动条导致的页面抖动
![页面抖动](https://user-images.githubusercontent.com/106876072/193528217-7d683827-7628-4c3d-9538-e752fa66dd7b.jpg)
![页面抖动_2](https://user-images.githubusercontent.com/106876072/193528238-1b1c7810-53be-4854-9285-dae93ba279fe.jpg)




1.原因:页面的内容高度小于VH高度，滚动条这时是隐藏状态，当切换到其他内容高度大于VH页面时，滚动条出现，导致页面抖动。

2.解决思路:设置 body {width: 100vw;}
