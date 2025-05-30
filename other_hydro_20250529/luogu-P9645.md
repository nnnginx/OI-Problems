## 题目描述
A $k$-hour clock is a day keeping method which follows the rules below:

- A day is divided into $k$ hours, where the $i$-th hour is called the $(i-1)$ o' clock;
- If it's $x$ o'clock now, it will be $(x+1)$ o'clock after $1$ hour if $0 \le x < k - 1$;
- If it's $(k - 1)$ o'clock now, it will be $0$ o'clock after $1$ hour.

We know that it's $x$ o'clock now, and after $y$ hours it will be $z$ o'clock. What's the value of $k$?


## 输入格式
There are multiple test cases. The first line of the input is an integer $T$ (about $10^5$), indicating the number of test cases. For each test case:

The first and only line contains three integers $x$, $y$ and $z$ ($0 \le x, z \le 10^9$, $1 \le y \le 10^9$).

## 输出格式
For each test case output one line containing one integer, indicating the value of $k$. Note that there must be $1 \le k \le 2 \times 10^9$. If there are multiple valid answers, you can print any of them; If there is no valid answer, print ``-1`` (without quotes) instead.

## 题目大意
给定三个数 $x,y,z$，求一个满足 $k>x,k>z$ 的数 $k$，使得 $x+y\equiv z\pmod k$。

```input1
4
11 18 5
3 49 4
1 9 1
1 3 10
```

```output1
12
24
3
-1
```

