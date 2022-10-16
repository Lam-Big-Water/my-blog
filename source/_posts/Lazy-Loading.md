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



# JavaScript 基础知识总结

1.一般来说，只有最简单的脚本才嵌入到 HTML 中。更复杂的脚本存放在单独的文件中。

使用独立文件的好处是浏览器会下载它，然后将它保存到浏览器的 缓存 中。

之后，其他页面想要相同的脚本就会从缓存中获取，而不是下载它。所以文件实际上只会下载一次。

这可以节省流量，并使得页面（加载）更快。

2.如果设置了 src 特性，script 标签内容将会被忽略。

一个单独的 <script> 标签不能同时有 src 特性和内部包裹的代码。
  
3.JavaScript 的变量命名有两个限制：

变量名称必须仅包含字母、数字、符号 $ 和 _。
  
首字符必须非数字。

区分大小写

留意保留字

4.未采用 use strict 下的赋值

一般，我们需要在使用一个变量前定义它。但是在早期，我们可以不使用 let 进行变量声明，而可以简单地通过赋值来创建一个变量。现在如果我们不在脚本中使用 use strict 声明启用严格模式，这仍然可以正常工作，这是为了保持对旧脚本的兼容。

5.数据类型

在 JavaScript 中有 8 种基本的数据类型（译注：7 种原始类型（primitive）和 1 种引用类型）。

JavaScript，被称为“动态类型”（dynamically typed）编程语言中有不同的数据类型，但是你定义的变量并不会在定义后，被限制为某一数据类型。

5.1Number类型

除了常规的数字，还包括所谓的“特殊数值（“special numeric values”）”也属于这种类型：Infinity、-Infinity 和 NaN。

Infinity 代表数学概念中的 无穷大 ∞。是一个比任何数字都大的特殊值。

NaN 代表一个计算错误。它是一个不正确的或者一个未定义的数学操作所得到的结果
NaN 是粘性的。任何对 NaN 的进一步数学运算都会返回 NaN

5.2BigInt类型

BigInt 类型是最近被添加到 JavaScript 语言中的，用于表示任意长度的整数。
目前 Firefox/Chrome/Edge/Safari 已经支持 BigInt 了，但 IE 还没有。

5.3String类型

JavaScript 中的字符串必须被括在引号（quotes）里。

新增反引号（Backticks）模板字符串（extended functionality）
它们允许我们通过将变量和表达式包装在 ${…} 中，来将它们嵌入到字符串中。

5.4Boolean类型

boolean 类型仅包含两个值：true 和 false。

5.5Null值

JavaScript 中的 null 仅仅是一个代表“无”、“空”或“值未知”的特殊值。

5.6undefined值

undefined 的含义是 未被赋值。
如果一个变量已被声明，但未被赋值，那么它的值就是 undefined

5.7symbol类型

symbol 类型用于创建对象的唯一标识符。

5.8Object类型

object 类型是一个特殊的类型。

其他所有的数据类型都被称为“原始类型”，因为它们的值只包含一个单独的内容（字符串、数字或者其他）。相反，object 则用于储存数据集合和更复杂的实体。

6.typeof运算符

typeof 是一个操作符

typeof 运算符返回参数的类型。当我们想要分别处理不同类型值的时候，或者想快速进行数据类型检验时，非常有用。

注意：

Math 是一个提供数学运算的内建 object。我们会在 数字类型 一节中学习它。此处仅作为一个 object 的示例。

typeof null 的结果为 "object"。这是官方承认的 typeof 的错误，这个问题来自于 JavaScript 语言的早期阶段，并为了兼容性而保留了下来。

typeof alert 的结果是 "function"，因为 alert 在 JavaScript 语言中是一个函数。
