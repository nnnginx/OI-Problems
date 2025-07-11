# AT_abc314_h [ABC314Ex] Disk and Segments

## 题目描述

在平面直角坐标系中，有 $N$ 条线段，第 $i$ 条的端点是 $(a_i,b_i)$ 和 $(c_i,d_i)$，任意线段不共点。

你要在平面上画一个圆，使得任意一条线段都和圆周或圆内部有至少一个公共点，求满足条件的圆的最小半径，绝对或相对误差不超过 $10^{-5}$。

## 输入格式

第一行一个整数 $N$，接着 $N$ 行每行四个整数 $a_i,b_i,c_i,d_i$。

## 输出格式

一行一个实数表示答案。

## 输入输出样例 #1

### 输入 #1

```
4
2 3 2 10
4 0 12 6
4 8 6 3
7 8 10 8
```

### 输出 #1

```
3.319048676309097923796460081961
```

## 输入输出样例 #2

### 输入 #2

```
20
0 18 4 28
2 21 8 21
3 4 10 5
3 14 10 13
5 9 10 12
6 9 10 6
6 28 10 18
12 11 15 13
12 17 12 27
13 17 20 18
13 27 19 26
16 1 16 13
16 22 19 25
17 22 20 19
18 4 23 4
18 5 23 11
22 16 22 23
23 15 30 15
23 24 30 24
24 0 24 11
```

### 输出 #2

```
12.875165712523887403637822024952
```

## 输入输出样例 #3

### 输入 #3

```
30
526 655 528 593
628 328 957 211
480 758 680 794
940 822 657 949
127 23 250 385
281 406 319 305
277 598 190 439
437 450 725 254
970 478 369 466
421 225 348 141
872 64 600 9
634 460 759 337
878 514 447 534
142 237 191 269
983 34 554 284
694 160 589 239
391 631 22 743
377 656 500 606
390 576 184 312
556 707 457 699
796 870 186 773
12 803 505 586
343 541 42 165
478 340 176 2
39 618 6 651
753 883 47 833
551 593 873 672
983 729 338 747
721 77 541 255
0 32 98 597
```

### 输出 #3

```
485.264732620930836460637042310401
```

## 说明/提示

* $2\leq N\leq 100$
* $0\leq a_i,b_i, c_i,d_i\leq1000\ (1\leq i\leq N)$
* $(a_i,b_i)\neq(c_i,d_i)\ (1\leq i\leq N)$