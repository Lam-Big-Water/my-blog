---
title: 懒加载
---
# 一.图片懒加载

## 图片懒加载的定义

展示那些需要展示给用户的图片，话句话说，就是只有用户浏览到的地方，才需要加载出图片。

## 图片懒加载的实现

1.不直接给img标签的src属性赋值，可以先给其data-src属性值赋值图片的地址

2.当图片到顶部的距离大于可视区域和滚动区域之和的时候，再将data-src的值赋值给src

---
## 使用IntersectionObserver API

![img-lazy-loading](https://user-images.githubusercontent.com/106876072/194594813-93c1b99c-75f9-40c0-bd4a-077643c7b52a.png)

## 封装

![lazy-loading-hooks](https://user-images.githubusercontent.com/106876072/194768795-eb92c5b0-2dbf-4891-8d2b-7b9f8fe09542.png)


