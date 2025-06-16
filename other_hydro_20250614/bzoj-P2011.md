## 题目描述

Georg 有个 MP3 Player，没有任何操作 $t$ 秒钟就会锁定，这时按下任意一个键就会变回没锁定的状态，但不会改变频道。只有在没锁定的状态下按键才有可能改变频道。MP3 的频道为 $0 \sim v_{max}$，如果现在是 $x$ 频道，若 $x < v_{max}$，在无锁状态下按 `+`，$x$ 就会加 $1$。若 $x>0$，在无锁状态下按 `-`，$x$ 就会减 $1$。Georg 忘记了 MP3 的 $t$ 是多少。他想通过一段操作试验一下。然后他就写下他的操作顺序和最后停留的频道 $v_2$，然后就给你了，你要求的是 $t$ 的最大值和 $t$ 在这个值的情况下，第一个操作前的频道 $v_1$ 的最大可能数。

## 输入格式

第一行：$n,v_{max},v_2$。$n$ 表示 Georg 操作了 $n$ 次；

以下 $n$ 行，每行第一个为字符 $c$，第二个为数字 $t_i$，表示 Georg 在 $t_i$ 秒按下了 $c$ 键。

## 输出格式

输出 $t$ 的最大值和 $t$ 在这个值的情况下，第一个操作前的频道 $v_1$ 的最大可能数。

若 $t$ 为无限大时经过这段操作最后能停在 $v_2$，则输出 `infinity`。

```input1
6 4 3
- 0
+ 8
+ 9
+ 13
- 19
- 24
```
```output1
5 4
```

## 样例说明 1

For $t=5$ the keys perform the following actions: `unlock, unlock, +, +, unlock, -`.
For any we would get $v_2 = 3$. Note that the output contains the largest possible $v_1$.
For the last two keystrokes will both be active, hence it will be impossible to have $v_2=3$.

```input2
3 10 10
+ 1
+ 2
+ 47
```
```output2
infinity
```
## 样例说明 2

If $v_1 = 10$ then for any $t$ we'll have $v_2 = 10$.

## 数据规模与约定

对于 $40\%$ 的数据，$n \leq 4\times10^3$。

对于 $70\%$ 的数据，$n \times v_{max}\leq 4\times 10^5$。

对于 $100\%$ 的数据，$2\leq n\leq 10^5$，$2\leq v_{max}\leq 5\times10^3$，$0 < c_i < 2\times 10^9$，$0\leq v_2 \leq v_{max}$，$x_i\in\{\texttt{+}, \texttt{-} \}$。