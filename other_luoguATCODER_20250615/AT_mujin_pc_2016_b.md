# AT_mujin_pc_2016_b ロボットアーム

## 题目描述

想象一只机器人手臂，将其看作是二维的一条线 $O-A-B-C$，其中 $O$ 这个点固定在原点 $(0,0)$。

如下图所示。

![](https://mujin-pc-2016.contest.atcoder.jp/img/other/mujin2016/arm_01.png)

现在，你可以改变 $\angle O,\ \angle A$ 和 $\angle B$ 的角度，但不可以改变任何线段的长度。

现在给定各条线段的长度，你需要计算 $C$ 能到达的范围总面积。

## 输入格式

$$l_{OA}\ l_{AB}\ l_{BC}$$

## 输出格式

输出 $C$ 可以到达的范围面积，误差不超过 $10^{-6}$ 都会视作正确答案。

**在最后输出换行。**

### 样例数据

**样例 1**

```
1 1 1
```

```
28.2743338823
```

解释：

![](https://mujin-pc-2016.contest.atcoder.jp/img/other/mujin2016/arm_02.png)

**样例 2**

```
3 1 1
```

```
75.3982236862
```

解释：

![](https://mujin-pc-2016.contest.atcoder.jp/img/other/mujin2016/arm_03.png)

**样例 3**

```
16 2 27
```

```
6107.2561185786
```

## 说明/提示

$1\le l_{OA},\ l_{AB},\ l_{BC}\le 100$

### 翻译贡献

@[hellolin](https://www.luogu.com.cn/user/751017) 译。