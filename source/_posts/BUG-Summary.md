---
title: 页面抖动
---
# 时有时无的滚动条导致的页面抖动

![呈现](https://user-images.githubusercontent.com/106876072/187362388-9a250220-2efa-4529-9905-81a2d1563984.jpg)


1.原因:页面的内容高度小于VH高度，滚动条这时是隐藏状态，当切换到其他内容高度大于VH页面时，滚动条出现，导致页面抖动。

2.解决思路: