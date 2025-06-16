## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/rfbq8b93.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/ripne4gf.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/37jmegj4.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/6l5xd1rh.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/qsdshz5j.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/821bcpy4.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/s2h64htt.png)

## 题目描述
给你 $n$ 个结点和 $m$ 条有向边，点编号为 $1,2,\dots,n$。每条边的颜色是黑色或者白色。一开始所有 $m$ 条边都是黑色的。

你需要进行 $q$ 次操作，有两种操作：

`1 k`：将第 $k$ 条边的颜色进行反转。

`2 u v`：询问是否能从 $u$ 只经过黑色的边走到 $v$。

## 输入格式
第一行有三个数 $n,m$ 和 $q$，表示点数，边数，操作数。

之后 $m$ 行，每行包含两个数 $u_i$ 和 $v_i$，表示有一条从 $u_i$ 到 $v_i$ 的有向边。

之后 $q$ 行，每行一个操作，格式如上述。

## 输出格式
对每个询问，如果可以从 $u$ 只经过黑色的边走到 $v$，则输出 `YES`，否则输出 `NO`。

```input1
5 6 7
1 2
1 3
2 4
3 4
3 5
4 5
2 1 5
2 2 3
1 3
1 4
2 1 4
1 3
2 1 5
```

```output1
YES
NO
NO
YES
```

## 提示
Idea：Claris，Solution：Claris，Code：Claris，Data：Claris

对于 $100\%$ 的数据，满足 $2 \leq n \leq 5\times 10^4$, $1\leq m,q\leq 10^5$，$1 \leq k \leq m$，$1 \leq u,v \leq n$, $u\neq v$。

