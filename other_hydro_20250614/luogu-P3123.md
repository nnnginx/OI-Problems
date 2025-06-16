## 题目描述
Farmer John and Bessie the cow love to exchange math puzzles in their free time.

The last puzzle FJ gave Bessie was quite difficult and she failed to solve it.

Now she wants to get even with FJ by giving him a challenging puzzle.

Bessie gives FJ the expression $(B+E+S+S+I+E)(G+O+E+S)(M+O+O)$, containing the seven variables $B,E,S,I,G,O,M$ (the "$O$" is a variable, not a zero).  For each variable, she gives FJ a list of up to 500 integer values the variable can possibly take.

She asks FJ to count the number of different ways he can assign values to the variables so the entire expression evaluates to a multiple of 7.

Note that the answer to this problem can be too large to fit into a 32-bit integer, so you probably want to use 64-bit integers (e.g., "long long"s in C or C++).

## 输入格式
The first line of the input contains an integer $N$.  The next $N$ lines each contain a variable and a possible value for that variable.  

Each variable will appear in this list at least once and at most 500 times. No possible value will be listed more than once for the same variable. All possible values will be in the range $-10^5$ to $10^5$.


## 输出格式
Print a single integer, giving the number of ways FJ can assign values to variables so the expression above evaluates to a multiple of 7.


## 题目大意
### 题目描述

Farmer John 和奶牛 Bessie 喜欢在空闲时间互相出数学谜题。

上一次 FJ 给 Bessie 出的谜题非常难，她没能解出来。

现在，她想通过给 FJ 出一个有挑战性的谜题来报复他。

Bessie 给 FJ 的表达式是 $(B+E+S+S+I+E)(G+O+E+S)(M+O+O)$，其中包含七个变量 $B,E,S,I,G,O,M$（"$O$" 是一个变量，不是零）。对于每个变量，她给 FJ 提供了一个最多包含 500 个整数值的列表，表示该变量可能取的值。

她要求 FJ 计算有多少种不同的方式可以为这些变量赋值，使得整个表达式的值是 7 的倍数。

注意，这个问题的答案可能太大，无法用 32 位整数表示，因此你可能需要使用 64 位整数（例如，C 或 C++ 中的 "long long"）。

### 输入格式

输入的第一行包含一个整数 $N$。接下来的 $N$ 行每行包含一个变量及其可能的值。

每个变量在这个列表中至少出现一次，最多出现 500 次。对于同一个变量，不会列出重复的可能值。所有可能的值都在 $-10^5$ 到 $10^5$ 的范围内。

### 输出格式

输出一个整数，表示 FJ 可以为变量赋值的方式数，使得上述表达式的值是 7 的倍数。

### 说明/提示

两种可能的赋值方式是：

$(B,E,S,I,G,O,M) = (2, 5, 7, 9, 1, 16, 19)$ -> 51,765

$(B,E,S,I,G,O,B) = (2, 5, 7, 9, 1, 16, 2)$ -> 34,510

```input1
10
B 2
E 5
S 7
I 10
O 16
M 19
B 3
G 1
I 9
M 2
```

```output1
2
```

## 提示
The two possible assignments are


(B,E,S,I,G,O,M) = (2, 5, 7, 9,  1, 16, 19) -> 51,765

(B,E,S,I,G,O,B) = (2, 5, 7, 9,  1, 16, 2 ) -> 34,510


