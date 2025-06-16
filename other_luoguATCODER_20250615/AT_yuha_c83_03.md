# AT_yuha_c83_03 Dendrogram - 樹形図

## 题目描述

## 题目背景
Nathan. O. Davis 是计算机科学系的学生。他正在为他所在部门名为“人工智能导论”的课程的最终作业编写一个层次聚类程序。
将一组对象划分为多个子集的过程，称为聚类。属于同一簇的对象根据某些标准被确定为相似。层次聚类是一种间接执行此操作的方法，它以称为树形图的树形结构处理一组对象。但是，在这个问题中，一组树也被视为树图。树形图表示对象之间的相似程度。树形图的示例如下所示。

![](https://atcoder.jp/img/other/yuha-c83/3_clean.png)

[图片没有的话，自己点击查看](https://atcoder.jp/img/other/yuha-c83/3_clean.png)

在上图中，终端叶子代表每个对象。水平线段表示将一组对象划分为两个或多个子组。属于不同子组的对象相似度低，属于同一子组的对象相似度高。这表明水平线位置越高，对象或属于该水平线的对象集合的相似度越低。举个例子，上图中从上数第二条水平线表示对象的集合被分成了三个簇。

Nathan 编写的程序可以输出系统发育树，但它包含两个错误。第一点是系统发育树是不连通的，即输出的系统发育树由多个树结构组成。我们不会在这个问题上处理这个问题。第二点是输出的系统发育树看起来很乱。具体来说，线段相交就像：

![](https://atcoder.jp/img/other/yuha-c83/3_dirty.png)

[图片没有的话，自己点击查看](https://atcoder.jp/img/other/yuha-c83/3_dirty.png)

它变得难以阅读。你的工作是编写一个程序，将 Nathan 的系统发育树作为输入并输出一个整洁的系统发育树。在这里，整洁的系统发育树被定义为除了接触点之外垂直和水平段不接触的树，并且终端叶数在字典序中最小。

## 输入格式

第一行三个整数 $N ( 1≤N≤100,000 )、 M ( 0≤M<N )、 Q ( 1≤Q≤1,000 , Q≤N )$。$N$ 是终端叶子的数量，$M$ 是水平线段的数量，$Q$ 是查询的数量。

接下来 $M$ 行，
- 每行给出第 $i$ 水平线段的信息：$Y_i,L_i$，其中 $Y_i$ 表示第 $i$ 条水平线的高度， $Y_i$ 越小，水平线高度越高（相似度越低）。$L_i$ 表示连接到第 $i$ 条水平线段的垂直线段数量。
- 紧接着会有 $V_1,V_2,…,V_{L_i}$ 共 $L_i$ 个数字，代表垂直线段编号，数据保证对于每条连接到同一条水平线段的垂直线段都有 $V_i ≠ V_j(1 \le i,j \le L_i,i≠j)$。

接下来 $Q$ 行，每行一个整数 $I_i$，表示查询整洁树中 $I_i$ 位置的垂直线段编号。

## 输出格式

对于每一个查询的 $I_i$，输出整洁树中 $I_i$ 位置上的垂直线段编号（注意位置从1开始）。

## 输入输出样例
### 输入#1
```
3 2 3
10 2 1 2
20 2 3 2
1
2
3
```
### 输出#1
```
1
2
3
```
[样例1解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample01.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample01.png)
### 输入#2
```
5 2 5
10 3 1 2 4
20 3 2 3 5
1
2
3
4
5
```
### 输出#2
```
1
2
3
5
4
```

[样例2解释图片](https://atcoder.jp/img/other/yuha-c83//3_sample02.png)
![](https://atcoder.jp/img/other/yuha-c83//3_sample02.png)
### 输入#3
```
4 1 4
10 2 1 4
1
2
3
4
```
### 输出#3
```
1
4
2
3
```
[样例3解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample03.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample03.png)
### 输入#4
```
4 3 4
30 2 1 4
20 2 2 4
10 2 3 4
1
2
3
4
```
### 输出#4
```
1
4
2
3
```
[样例4解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample04.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample04.png)
### 输入#5
```
4 3 4
10 2 1 4
20 2 2 4
30 2 3 4
1
2
3
4
```
### 输出#5
```
1
2
3
4
```
[样例5解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample05.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample05.png)
### 输入#6
```
4 3 4
10 2 1 2
15 2 1 4
20 2 2 3
1
2
3
4
```
### 输出#6
```
1
4
2
3
```
[样例6解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample06.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample06.png)
### 输入#7
```
3 2 3
10 2 2 3
20 2 1 2
1
2
3
```
### 输出#7
```
1
2
3
```
[样例7解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample07.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample07.png)
### 输入#8
```
1 0 1
1
```
### 输出#8
```
1
```
[样例8解释图片](https://atcoder.jp/img/other/yuha-c83/3_sample08.png)
![](https://atcoder.jp/img/other/yuha-c83/3_sample08.png)