## 题目描述
Kotori is practicing making fireworks for the upcoming hanabi taikai$^1$. It takes her $n$ minutes to make a single firework, and as she is not really proficient in making fireworks, each firework only has a probability of $p \times 10^{-4}$ to be perfect.

After she finishes making a firework, she can just start making the next firework, or take $m$ minutes to light all the remaining fireworks finished before. If there is at least one perfect firework among the lit ones, she will be happy and go to rest. Otherwise, she will continue practicing. Can you tell her the minimum expected practicing time before she goes to rest if she takes the optimal strategy?

Notice that no matter how many fireworks remain, it always takes $m$ minutes to light them all.

$^1$ Hanabi taikai: Romaji of the Japanese word ``花火大會``, which means the firework... err... party?

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 10^4$) indicating the number of test cases. For each test case:

The first and only line contains three integers $n$, $m$ and $p$ ($1 \le n, m \le 10^9$, $1 \le p \le 10^4$).

## 输出格式
For each test case, output one line containing one number indicating the minimum expected practicing time.

Your answer will be considered correct if and only if the absolute or relative error does not exceed $10^{-4}$.

## 题目大意
Kotori 正在制作烟花。她制作一支烟花需要 $n$ 分钟，每支烟花有 $p\times 10 ^ {-4}$ 的概率是完美的。

当 Kotori 制作好一支烟花时，她可以选择继续制作，也可以选择用 $m$ 分钟点燃所有烟花。如果其中有完美的烟花，那么她会很开心，并停下来休息，否则她会继续制作烟花。你能告诉她在最优策略下，最少期望多长时间才能停下来休息吗？

注意，无论已经制作好了多少支烟花，Kotori 都需要 $m$ 分钟将它们点燃。

多组数据，$1\leq T, p\leq 10 ^ 4$，$1\leq n, m\leq 10 ^ 9$。要求相对误差或绝对误差不超过 $10 ^ {-4}$。

```input1
3
1 1 5000
1 1 1
1 2 10000
```

```output1
4.0000000000
10141.5852891136
3.0000000000
```

