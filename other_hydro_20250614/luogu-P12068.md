## 题目背景
搬运自 [2013 年清华大学信息学邀请赛](https://gitlink.org.cn/thusaa/thoi2013)。

upd 2025.4.7 10:20：本题 spj 已修复。

udp 2025.4.16 19:19：添加了一组 Hack 数据，位于 Subtask #1。感谢 @[AL8624](/user/913226) 的贡献。

## 题目描述
小胜是宇宙飞艇神舟 $100$ 号的指挥官，正在指挥神舟 $100$ 号进行航行任务。

神舟 $100$ 号上一共有 $n$ 个能够在水平方向产生推力的引擎（至于垂直的第三维方向，小胜对此并不关心），其中第 $i$ 个引擎能够使飞艇获得的水平速度为 $\overrightarrow{p_i}=(x_i,y_i)$。由于采用了特殊技术，飞艇在运行过程中不会发生旋转。

为了能够尽快的执行任务，小胜希望你帮助他解决下列问题：
1. 飞艇利用这些引擎在 $\overrightarrow{q}=(x_q,y_q)$ 方向上获得的最大分速度是多少？
2. 飞艇利用这些引擎所能获得的最大速度是多少？
3. 飞艇恰好使用 $k$ 个引擎，所能获得的最大速度是多少？

为了方便表达，对于问题 $1$，请输出最大分速度与 $|\overrightarrow{q}|$（$\overrightarrow{q}$ 的模长，即 $\sqrt{x_q^2+y_q^2}$）的乘积；对于问题 $2$ 和问题 $3$，请输出最大速度的平方。

## 输入格式
第一行包含一个正整数 $n$，表示引擎的个数。

第二行包含两个整数 $x_q$ 和 $y_q$，表示方向 $\overrightarrow{q}=(x_q,y_q)$。

接下来 $n$ 行，每行包含两个整数 $x_i$ 和 $y_i$，表示第 $i$ 个引擎所能提供的速度为 $\overrightarrow{p_i}=(x_i,y_i)$。

## 输出格式
第一行为一个整数，表示神舟 $100$ 号在 $\overrightarrow{q}$ 方向上最大分速度与 $|\overrightarrow{q}|$ 的乘积的值。

第二行为一个整数，表示通过这 $n$ 个引擎所能得到的最大速度值的平方。

第三行包含 $n$ 个用空格隔开的整数，其中第 $k$ 个整数表示恰好开启 $k$ 个引擎所能得到的最大速度的平方。

```input1
4
1 1
0 1
1 0
-1 0
0 -1
```

```output1
2
2
1 2 1 0
```

```input2
8
1 1
-1 0
0 1
1 2
2 3
0 -1
0 -2
3 -3
3 -3
```

```output2
9
117
18 72 100 117 106 97 90 73
```

## 提示
### 【对样例的说明】

对于样例 1，要获得在 $\overrightarrow{q}=(1,1)$ 方向的最大分速度，最佳方案是打开前两个引擎，而打开这两个引擎也可以使得飞艇获得最大速度。

对于样例 2，要使得飞艇获得在 $\overrightarrow{q}=(1,1)$ 方向的最大分速度，需要打开 $2,3,4$ 号引擎，而要使得飞艇获得最大速度，则需要打开 $5,6,7,8$ 号引擎。

### 【数据规模与约定】

$25\%$ 的数据满足 $n\le300$。

$50\%$ 的数据满足对于任意 $1\le i<j<k\le n$，$(x_i,y_i),(x_j,y_j),(x_k,y_k)$ 三点不共线。

$100\%$ 的数据满足 $3\le n\le1000$，$0<|\overrightarrow{q}|\le1000$ 并且对于任意 $1\le i\le n$，$|\overrightarrow{p_i}|>0,|x_i|\le 10^5,|y_i|\le 10^5$。

### 【数学小贴士】

对于两个二维向量与 $\overrightarrow{u}=(x_u,y_u)$ 与 $\overrightarrow{v}=(x_v,y_v)$，我们用 $u\cdot v$ 表示向量的内积，用 $u\times v$ 表示向量的叉积。向量的内积和叉积的计算满足如下恒等式：

$$\overrightarrow{u}\cdot \overrightarrow{v}=\overrightarrow{v}\cdot \overrightarrow{u}=x_ux_v+y_uy_v=|\overrightarrow{u}|| \overrightarrow{v}|\cos \theta$$

$$\overrightarrow{u}\times \overrightarrow{v}=-\overrightarrow{v}\times \overrightarrow{u}=x_uy_v-x_vy_u=|\overrightarrow{u}|| \overrightarrow{v}|\sin \theta$$

这里 $\theta$ 表示向量 $\overrightarrow{u}$ 和 $\overrightarrow{v}$ 的夹角大小。


