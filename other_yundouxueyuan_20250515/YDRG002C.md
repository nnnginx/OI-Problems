## 题目背景

![Snipaste\_2023-08-07\_20-25-01.png](https://img.macesuted.moe/43b8403457e60dc3a19d2e4ca0df975a/5fb1f8b2a75a7.png)

## 题目描述

在这个题目中，你需要解决这样一个问题：

给定一个长度为 $w$（$w=60$）的 $01$ 序列 $a_{0,1,2\dots,w-1}$，你需要求出他有多少个子区间的区间和等于区间长度。

为了压缩读入量，序列 $a$ 将采用特殊的方法生成，具体的，你将读入一个正整数 $x$（$x< 2^{w}$） 表示 $a$，其中 $x=a_0\times 2^{0}+a_1\times 2^1\dots a_{w-1}\times 2^{w-1}$。

本题有多组询问，共 $q$（$q\le 5\times 10^7$） 次，将采用读入和随机相结合的方式生成，具体方法见输入格式。

## 输入格式

第一行四个正整数 $q,k,a,c$，其中 $q$ 的含义见题目描述，$k,a,c$ 用以读入数据，具体方法如下：

该题所有 $q$ 次询问中，前 $k$ 次询问的 $x_1,x_2,\dots,x_k$ 在输入中给定，每行一个，从第 $k+1$ 次询问开始的 $x_i=(\operatorname{xorshift}(x_{i-1})+a)\bmod c$。其中 $\operatorname{xorshift}$ 的具体含义将在下方以代码形式给出。

保证 $c\leq 2^w$。

$\operatorname{xorshift}$ 代码片段如下：

```cpp
unsigned long long xorshift(int X){
	X ^= X << 13; X ^= X >> 17; X ^= X << 5; return X;
}
```

读入模板，保证该读入模板耗时小于 $\text{600 ms}$。

```cpp
#include<bits/stdc++.h>
unsigned long long a, c, x;
int q, k;
namespace Read{
	int cnt = 0; unsigned long long X;
	unsigned long long read(){
		if(++ cnt <= k) {std :: cin >> X; return X;}
		else {X ^= X << 13; X ^= X >> 17; X ^= X << 5; return X = (X + a) % c;}
	}
}
int main(){
	std :: ios :: sync_with_stdio(false); std :: cin.tie(0);
	std :: cin >> q >> k >> a >> c; 
	for(int i = 1; i <= q; i ++){
		x = Read :: read();
		/*
			Write your code.
		*/
	}
}
```

## 输出格式

为了减小输出量，记第 $i$ 次询问的答案为 $p_i$，你只需要输出 $(1\times p_1)\oplus (2\times p_2)\oplus\dots (q\times p_q)$ 的值。其中 $\oplus$ 表示二进制异或操作。

## 样例 #1

### 样例输入 #1

```
1 1 1 1
12345678910
```

### 样例输出 #1

```
59
```

### 数据范围与约定

本题采用捆绑测试。

对于 $100\%$ 的数据保证 $k\le10^6, q\leq5\times 10^7$。

| 子任务编号| $q=$ | $k\leq$ |分数|
| :---: | :---: | :---: | :---: |
| $1$ | $5\times 10^6$ | $10^6$ |$30$|
| $2$ | $5\times 10^7$ | $10^6$ |$70$|

