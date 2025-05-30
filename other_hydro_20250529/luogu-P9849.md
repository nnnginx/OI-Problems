## 题目描述
Once again, Xingqiu hides Chongyun's ice cream into a box with a strange lock. Liyue's summer has been always very hot and Chongyun suffers more because of his excessive yang (positive) energy, so he needs that ice cream desperately.

![](https://cdn.luogu.com.cn/upload/image_hosting/2dtcr426.png)

There are two integers $a$ and $b$ on the lock. Chongyun can perform the following three types of operations any number of times:
- Minus $1$ from both $a$ and $b$;
- Plus $1$ to both $a$ and $b$;
- Divide both $a$ and $b$ by one of their common $\textbf{prime}$ factor (that is to say, divide them by a $\textbf{prime}$ $g$ where $a$ and $b$ are both divisible by $g$).

The box will be unlocked if either $a$ or $b$ or both become $1$. To help Chongyun gets the ice cream back as quickly as possible, please tell him the minimum number of operations needed to unlock the box.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 300$) indicating the number of test cases. For each test case:

The first and only line contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$, $a \ne b$).

## 输出格式
For each test case output one line containing one integer indicating the minimum number of operations to make $a$ or $b$ or both equal $1$.

## 题目大意
## 题目描述
有 $T$ 个盒子，每盒子上有一个锁，锁上有两个整数 $a$ 和 $b$。你可以对这个锁做若干次以下 3 种操作：

- $a$ 和 $b$ 分别减去 $1$
- $a$ 和 $b$ 分别增加 $1$
- $a$ 和 $b$ 分别除以它们共同的素数因子

如果 $a$ 或 $b$ 或两者都变为 $1$，盒子就会解锁。请你编写一个程序，计算每个盒子的锁打开的最少步骤数量。

## 输入格式
第一行输入一个整数 $T(1≤T≤300)$。

接下来 $T$ 行，每行输入 $a$ 和 $b$，表示每个盒子的锁的信息。

## 输出格式  

共输出 $T$ 行，每行输出对应盒子解锁的最少步骤。

```input1
5
4 7
9 8
32 84
11 35
2 1

```

```output1
2
7
5
4
0

```

## 提示
For the first sample test case, the optimal way is $(4, 7) \rightarrow (3, 6) \rightarrow (1, 2)$.

For the second sample test case, the optimal way is to apply the first type of operation $7$ times.

For the third sample test case, the optimal way is $(32, 84) \rightarrow (16, 42) \rightarrow (15, 41) \rightarrow (14, 40) \rightarrow (13, 39) \rightarrow (1, 3)$.

For the fourth sample test case, the optimal way is $(11, 35) \rightarrow (12, 36) \rightarrow (6, 18) \rightarrow (2, 6) \rightarrow (1, 3)$.

