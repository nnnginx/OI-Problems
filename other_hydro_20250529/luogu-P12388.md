## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/q0ae6v6a.png)

（图：某位不愿透露姓名的热心 /ˈfɜri/ 网友）

## 题目描述
定义：
$$f(n)=\sum_{i=1}^n\sum_{j=1}^n[\operatorname{popcount}(i+j)\gcd(i,j)=\max(i,j)]$$
其中 $\operatorname{popcount}(x)$ 是 $x$ 在二进制下 $1$ 的个数，$\gcd(i,j)$ 是 $i,j$ 的最大公约数。

现在给定正整数 $n$，你需要求出 $f(1)\oplus f(2)\oplus\cdots\oplus f(n)$ 的值。其中 $\oplus$ 是按位异或。

## 输入格式
一行一个正整数 $n$。

## 输出格式
一行一个自然数，表示 $f(1)\oplus f(2)\oplus\cdots\oplus f(n)$ 的值。

```input1
10
```

```output1
13
```

```input2
10000
```

```output2
3159
```

## 提示
**本题采用捆绑测试。**

- Subtask 1 (10pts)：$n\le 10$。
- Subtask 2 (10pts)：$n\le 10^3$。
- Subtask 3 (20pts)：$n\le 10^5$。
- Subtask 4 (30pts)：$n\le 10^6$。
- Subtask 5 (30pts)：$n\le 10^7$。

对于全部数据，$1\le n\le 10^7$。

