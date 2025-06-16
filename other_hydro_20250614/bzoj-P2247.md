

## 题目描述
> In the downtown of Bucharest there is a very big bank with a very big vault. Inside the vault there are $n$ very big boxes numbered from $1\sim n$. Inside the box with number $k$ there are $k$ very big diamonds, each of weight $W_k$ and cost $C_k$. 

> John and Brus are inside the vault at the moment. They would like to steal everything, but unfortunately they are able to carry diamonds with the total weight not exceeding $m$. 

> Your task is to help John and Brus to choose diamonds with the total weight less than or equal to $m$ and the maximal possible total cost.

## 中文翻译

在 Bucharest 市的市区里有一个很大的银行，银行的金库中有标号为 $1\sim n$ 的 $n$ 种盒子，第 $k$ 个盒子中有 $k$ 个重量为 $w_k$，价值为 $c_k$ 的钻石。

John 和 Brus 正在金库中行窃，他们本想带走所有钻石，可惜他们的背包容量只有 $m$，换句话说，设 $S$ 为他们带走的钻石标号集合，那么 $S$ 需满足

$$
\sum_{k\in S} w_k \le m
$$

你需要帮助 John 和 Brus，使得在满足这个条件下，最大化

$$
\sum_{k\in S} c_k
$$

## 输入格式
>The first line contains single integer $T$ – the number of test cases. Each test case starts with a line containing two integers $n$ and $m$ separated by a single space. The next line contains $n$ integers $w_k$ separated by single spaces. The following line contains $n$ integers $c_k$ separated by single spaces.

第一行一个整数 $T$，表示数据组数。

对于每组数据，第一行包括两个正整数 $n,m$。

接下来一行 $n$ 个正整数，第 $i$ 个整数表示 $w_i$。

接下来一行 $n$ 个正整数，第 $i$ 个整数表示 $c_i$。
## 输出格式
>For each test case print a single line containing the maximal possible total cost of diamonds.

对每组数据，输出对应的最大价值。

```input1
2 
2 4 
3 2 
5 3 
3 100 
4 7 1 
5 9 2

```
```output1
6 
29

```

## 提示
$1\le T\le 74,1\le n\le 15,1\le w_i,c_i,m\le 10^9$

## 题目来源
Seerc2009


