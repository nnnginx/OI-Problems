## 题目背景

众所周知，应急食品派蒙是旅行者伙伴中最好的银色飞天飘浮灵，也是机械宠物中最好的提瓦特导游——但是派蒙学历太低了！

为了帮助这只飞天小堇瓜升学，身为旅行者的你开始向她传授信息学竞赛的奥义。但没想到，虽然学了半天的 OI 没学会，派蒙最终却对线性代数有了很深刻的领悟。

因此，某天她出了这道题，打算考考你哦~

（诶，什么啊！旅行者又说派蒙写的题目背景逻辑不通顺了？好可恶啊！）

## 题目描述

派蒙给了你两个长度均为 $n$ 的 $01$ 序列 $\{a_n\}$ 和 $\{b_n\}$  ，她希望你能够和枫丹的水元素共鸣，生成一个矩阵 $\{c_{n,n}\}$。

其中生成的规则为：

$$
c_{i,j}=a_i\times b_j
$$

接下来，派蒙又随手掏出了一个 $k$ 。她想考考你，矩阵 $c_{n,n}$ 内，究竟有多少个**连续子矩阵**满足其中有 $k$ 个 $1$ 呢？

## 输入格式

输入的第一行有两个整数 $n,k$ 表示 $01$ 序列长以及目标子矩阵 $1$ 的个数。

第二行有一行 $n$ 个整数表示序列 $a$。

第三行有一行 $n$ 个整数表示序列 $b$。

## 输出格式

输出一行一个整数表示符合题意的子矩阵个数。由于答案可能过大，你需要输出的是答案除以质数 $998244353$ 的余数。

## 样例 #1

### 样例输入 #1

```
4 4
0 1 1 1
1 0 1 0
```

### 样例输出 #1

```
6
```

### 提示与说明

【样例解释】

如图，取蓝色字部分、米色背景部分、两个粗线框内部，以及小粗线框加上紫色或绿色的 $0$ 构成的矩阵均符合题意。

![](https://cdn.luogu.com.cn/upload/image_hosting/1zntkw51.png)![](https://cdn.luogu.com.cn/upload/image_hosting/xrgphyq5.png)

【数据规模与限制】

对于 $20\%$ 的数据，有 $1\leq n\leq 500$ 。

对于 $40\%$ 的数据，有 $1\leq n\leq 5000$。

对于额外 $10\%$ 的数据，有 $1\leq k \leq 4$ 。

对于额外 $10\%$ 的数据，有 $\forall 1\leq i\leq n,a_i=b_i$ 。

对于全部 $100\%$ 的数据，有 $1\leq n\leq 3\times 10^5,1\leq k\leq 10^{12}$。

“弦形袋鼠是什么啊，听起来好好吃啊\~旅行者，你能不能用甜甜花酿鸡的做法做一道啊\~拜托啦~~~”

