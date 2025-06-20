# AT_aising2020_f Two Snuke

## 题目描述

给你一个整数 $N$。你的任务是选择整数 $s_1, s_2, n_1, n_2, u_1, u_2, k_1, k_2, e_1, e_2$，这些整数需要满足以下六个条件：

1. $0 \leq s_1 < s_2$
2. $0 \leq n_1 < n_2$
3. $0 \leq u_1 < u_2$
4. $0 \leq k_1 < k_2$
5. $0 \leq e_1 < e_2$
6. $s_1 + s_2 + n_1 + n_2 + u_1 + u_2 + k_1 + k_2 + e_1 + e_2 \leq N$

对于所有满足以上条件的 $(s_1, s_2, n_1, n_2, u_1, u_2, k_1, k_2, e_1, e_2)$ 组合，计算 $(s_2 - s_1)(n_2 - n_1)(u_2 - u_1)(k_2 - k_1)(e_2 - e_1)$ 的值，并将这些结果的总和对 $10^9 + 7$ 取模。

问题涉及 $T$ 个测试用例，请分别计算每个测试用例的结果。

## 输入格式

输入以以下形式通过标准输入提供：

> $T$  
> $\mathrm{case}_1$  
> $\vdots$  
> $\mathrm{case}_T$

每个测试用例由一个整数 $N$ 组成。

## 输出格式

输出结果为 $T$ 行。每一行对应一个测试用例的答案。

## 输入输出样例 #1

### 输入 #1

```
4
4
6
10
1000000000
```

### 输出 #1

```
0
11
4598
257255556
```

## 说明/提示

- 所有输入均为整数。
- $1 \leq T \leq 100$
- $1 \leq N \leq 10^9$

### 示例解释

- 当 $N = 4$ 时，没有满足条件的整数组合，因此结果为 $0$。
- 当 $N = 6$ 时，满足条件的整数组合有以下 $6$ 种：
  - $(0, 1, 0, 1, 0, 1, 0, 1, 0, 1)$
  - $(0, 2, 0, 1, 0, 1, 0, 1, 0, 1)$
  - $(0, 1, 0, 2, 0, 1, 0, 1, 0, 1)$
  - $(0, 1, 0, 1, 0, 2, 0, 1, 0, 1)$
  - $(0, 1, 0, 1, 0, 1, 0, 2, 0, 1)$
  - $(0, 1, 0, 1, 0, 1, 0, 1, 0, 2)$

其中，$(s_2 - s_1)(n_2 - n_1)(u_2 - u_1)(k_2 - k_1)(e_2 - e_1)$ 的结果为 $1$ 的组合有 $1$ 种，结果为 $2$ 的组合有 $5$ 种，故答案为 $11$。

注意结果需对 $10^9 + 7$ 取模。

 **本翻译由 AI 自动生成**