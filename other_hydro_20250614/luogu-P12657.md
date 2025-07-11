## 题目背景
试题来源：<https://koi.or.kr/archives/>。中文翻译做了少量本土化修改。

按照[署名—非商业性使用—相同方式共享 4.0 协议国际版](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh-hans)进行授权。

## 题目描述
如图所示，第 1 行有 1 个数，第 2 行有 2 个数，……，第 $N$ 行有 $N$ 个数，构成一个正三角形。给定两个这样的正三角形 $A$ 和 $B$，每个位置上的数为 0 或 1。

![](https://cdn.luogu.com.cn/upload/image_hosting/9z381rzh.png)

你可以对正三角形进行顺时针或逆时针方向的 $120^\circ$ 旋转，也可以进行左右对称变换。

例如，将图中的正三角形 $A$ 进行旋转后可以得到如下的正三角形。

![](https://cdn.luogu.com.cn/upload/image_hosting/gt35kinw.png)

将 $A$ 进行对称变换后可以得到如下的正三角形。

![](https://cdn.luogu.com.cn/upload/image_hosting/uf9lbcxb.png)

两个正三角形的“差异”定义为：将它们重叠后，数值不同的位置的数量。

例如，若将正三角形 $A$ 和 $B$ 重叠，在第 2 行最左侧，以及第 3 行的最左侧和最右侧位置的数值不同，因此 $A$ 和 $B$ 的差异为 3。

但若将 $A$ 逆时针旋转 $120^\circ$ 后再与 $B$ 重叠，仅在第 3 行从左起第 2 个位置的数值不同，这时差异为 1。

给定两个正三角形 $A$ 和 $B$。你可以对 $A$ 进行任意次数的旋转或对称操作。你也可以选择不进行任何变换。操作次数不限。

请将 $A$ 变换为与 $B$ 差异最小的形态，并输出此时的最小差异值。

## 输入格式
第一行包含一个整数 $N$，表示三角形的大小。

接下来的 $N$ 行表示三角形 $A$ 的内容。第 $i$ 行包含 $i$ 个整数，按从左到右的顺序给出，对应第 $i$ 层的数据。

再接下来的 $N$ 行表示三角形 $B$ 的内容。第 $i$ 行同样包含 $i$ 个整数，按从左到右的顺序给出，对应第 $i$ 层的数据。

## 输出格式
输出一个整数，表示将 $A$ 变换为与 $B$ 差异最小时的最小差异值。


```input1
3
0
1 0
1 0 0
0
0 0
0 0 1
```

```output1
1
```

```input2
4
0
1 1
1 0 0
1 0 0 0
0
0 0
0 0 1
1 1 1 0
```

```output2
0
```

```input3
4
0
1 0
0 0 1
1 1 0 0
0
0 1
0 0 0
0 1 1 1
```

```output3
2
```

## 提示
**样例 1 说明**

将 $A$ 逆时针旋转 $120^\circ$ 后，仅有一个位置与 $B$ 不同，差异为 1。还有其他方式也可以使差异为 1。

**限制条件**

- 所有给定的数值均为整数。
- $1 \leq N \leq 10$
- $A$ 和 $B$ 中每个位置的数值仅为 0 或 1。

**子问题**

1. （5 分）$A$ 中所有数值相同。换言之，$A$ 中所有位置均为 0 或均为 1。
2. （10 分）$N \leq 2$
3. （40 分）仅考虑旋转操作即可得到最优解。
4. （45 分）无额外限制。

翻译由 ChatGPT-4o 完成

