## 题目描述
Farmer John has purchased a new machine that is capable of planting grass within any rectangular region of his farm that is "axially aligned" (i.e., with vertical and horizontal sides).  Unfortunately, the machine malfunctions one day and plants grass in not one, but N (1 <= N <= 1000) different rectangular regions, some of which may even overlap.

Given the rectangular regions planted with grass, please help FJ compute the total area in his farm that is now covered with grass.

在一个笛卡尔平面坐标系里（则 $X$ 轴向右是正方向，$Y$ 轴向上是正方向），有 $N\ (1 \le N \le 1000)$ 个矩形，第 $i$ 个矩形的左上角坐标是 $(x_1,y_1)$，右下角坐标是 $(x_2,y_2)$。问这 $N$ 个矩形所覆盖的面积是多少？

注意：被重复覆盖的区域的面积只算一次。

## 输入格式
第一行，一个整数 $N\ (1 \le N \le 1000)$。

接下来有 $N$ 行，每行描述一个矩形的信息，分别是矩形的 $x_1,y_1,x_2,y_2(-10^8 \le x_1,y_1,x_2,y_2 \le 10^8)$。


## 输出格式
一个整数，被 $N$ 个矩形覆盖的区域的面积。


```input1
2
0 5 4 1
2 4 6 2

```

```output1
20
```

