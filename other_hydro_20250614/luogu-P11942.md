## 题目背景
版权信息：译自 [2025年度 国际情报 올림피아드 (Olympiad) 代表学生 选拔考试](https://www.ioikorea.or.kr/archives/ioitst/2025/) R1T1。[[CC BY-NC-SA 4.0](http://creativecommons.org/licenses/by-nc-sa/4.0/)]

---

由于洛谷评测系统的限制，本题将仅执行一次。请注意多测清空。

**使用全局变量来达成「绕过交互库传递信息，以获取大于 $0$ 分」的目的，将被视为作弊。**

你需要在文件头加入以下内容：

```cpp
void select(int x, int y);
```


## 题目描述

**这是一道通信题。交互库是非自适应（non-adaptive）的。** 
 本题中，下标默认为 $\textsf{0-index}$。

Alice 有一个 $n\times n$ 的 $01$ 矩阵 $A$，满足以下条件：

- **不存在** $0\le i_1\lt i_2\lt n$，$0\le j_1\lt j_2\lt n$ 使得 $\textcolor{red}{A_{i_1,j_1}=A_{i_2,j_2},A_{i_1,j_2}=A_{i_2,j_1},A_{i_1,j_1}\neq A_{i_1,j_2}}$ 均成立。

Alice 要把这个矩阵传递给 Bob。出于安全考虑，通信程序如下：

- Alice 从 $n^2$ 个元素中选择若干个；
- 交互库有两个隐藏的 $0\sim n-1$ 的排列 $p,q$；
- Bob 会得到一个 $n\times n$ 的矩阵 B。对于 Alice 选择的每个元素 $(i,j)$，都有 $B_{p_i,q_j}=A_{i,j}$；对于未选择的 $(i,j)$，有 $B_{p_i,q_j}=-1$。

Bob 要将 $B$ 矩阵中的 $-1$ 用 $0$ 或 $1$ 填充，使得 $\forall 0\le i,j\lt n$，都有 $B_{p_i,q_j}=A_{i,j}$ 成立。

### 实现细节

**这是一道通信题。交互库是非自适应（non-adaptive）的。** 

你不需要，也不应该实现 main 函数。禁止访问标准输入/输出流（`stdin`，`stdout`）。


你需要在文件头加入以下内容：

```cpp
void select(int x, int y);
```



你可以调用以下的函数：

```cpp
void select(int i, int j);
```

- 你需要保证 $0\le i,j\lt n$。
- 令该函数被调用的**总次数**为 $k$。

你需要实现以下的函数：

```cpp
void send(vector<vector<int>> A);
```

- 参数 `A`：一个长度为 $n$ 的二维 `vector`，其中每个元素都是一个长度为 $n$ 的 `vector<int>`。
- 在这个函数中，你应当调用 `select` 函数选择你想要传输的元素。
    - 调用 `select` 的次数不得超过 $n^2$。

```cpp
vector<vector<int>> reconstruct(vector<vector<int>> B);
```

对于 `send` 中给定的矩阵 $A$，这里参数 `B` 满足以下条件：

- `B` 是和 `A` 形状相同的二维 `vector`；
- $p,q$ 是交互库中隐藏的 $0\sim n-1$ 的排列；
- $\forall 0\le i,j\lt n$：
    - 若调用过 `select(i,j)`，则 $B_{p_i,q_j}=A_{i,j}$；
    - 否则，$B_{p_i,q_j}=-1$。
- 返回值 `C` 必须满足：
    - $\forall 0\le i,j\lt n$，都有 $C_{p_i,q_j}=A_{i,j}$ 成立。

### 注意事项

- `send` 中对 `select` 的调用，以及 `reconstruct` 的返回值**应当只依赖于给定参数的值**。若以相同参数多次调用时行为不一致，则会被判定为 $\text{Wrong Answer}$。
- 在交互库中，排列 $p,q$ 是**预先确定的**，**非适应性的**。但是你无法直接访问它们。
    - 在 Sample Grader 中，$p,q$ 会作为输入给出。
- **每个测试点中含有多组独立的测试数据**，每组数据会依次调用 `send` 和 `reconstruct` 恰好一次。
    - 我们不保证每组数据都按顺序运行，但保证函数调用及返回值的逻辑符合题目描述。
- 实际使用的 Grader 与 Sample Grader 的行为不同。请勿依赖 Sample Grader 的特定行为。
- 本题用时定义为 `send` 和 `reconstruct` 用时之和，内存使用量不大于两者使用的峰值内存之和。


## 输入格式
**本题单个测试点内含有多组测试数据。**

Sample Grader 输入格式如下：

> $n$\
> $A_{0,0}$ $A_{0,1}$ $\cdots$ $A_{0,n-1}$\
> $A_{1,0}$ $A_{1,1}$ $\cdots$ $A_{1,n-1}$\
> $\vdots$ \
> $A_{n-1,0}$ $A_{n-1,1}$ $\cdots$ $A_{n-1,n-1}$\
> $p_0$ $p_1$ $\cdots$ $p_{n-1}$\
> $q_0$ $q_1$ $\cdots$ $q_{n-1}$

## 输出格式

Sample Grader 输出格式如下：

1. 如果调用了不满足 $0 \leq i, j \leq n-1$ 的 `select(i, j)`，则输出一行 `Wrong Answer [1]`。  
2. 如果 `select` 的调用总次数 $k$ 超过 $n^2$，则输出一行 `Wrong Answer [2]`。  
3. 如果 `reconstruct` 的返回值 $C$ 的维度或元素数量与 $B$ 不一致，则输出一行 `Wrong Answer [3]`。  
4. 如果 $C$ 未满足条件 $C_{p_i,q_j}=A_{i,j}$，则输出一行 `Wrong Answer [4]`。  
5. 以上错误均未发生时，输出调用 `select` 的次数，格式为 `k: 10`。  

若检测到错误（输出任何 `Wrong Answer`），示例评测系统将立即终止运行。  


**注意：实际使用的 Grader 与 Sample Grader 的行为不同。请勿依赖 Sample Grader 的特定行为。**

```input1
3
1 1 1
1 1 0
0 1 0
2 1 0
0 1 2
```

```output1
k: 4
```

## 提示

#### 样例交互 $1$

$n=3$，$A=\begin{bmatrix}1 & 1 & 1 \\1 & 1 & 0 \\ 0 & 1 & 0\end{bmatrix}$，$p=[2,1,0]$，$q=[0,1,2]$。

交互库调用 `send`：

```cpp
send([1, 1, 1], [1, 1, 0], [0, 1, 0])
```

`send` 调用 `select` 函数：

```cpp
select(0,1)
select(0,2)
select(1,0)
select(2,2)
```

随后交互库调用 `reconstruct` 函数：

```cpp
reconstruct([[-1, -1, 0], [1, -1, -1], [-1, 1, 1]])
```

`reconstruct` 函数返回 `[[0, 1, 0], [1, 1, 0], [1, 1, 1]]`，被判定为 $\text{Accepted}$。

### 数据范围

- $1\le n\le 500$。
- $\sum n^2\le 10^6$。

### 子任务

- $\text{Subtask 0 (0 pts)}$：样例。
- $\text{Subtask 1 (12 pts)}$。

    - $\forall 0\le i,j\lt n$，$A_{i,j}=1\iff i\le j$。

- $\text{Subtask 2 (35 pts)}$。

    - 这个矩阵形如直方图（히스토그램 형태，histogram structure）。
    - 换言之，$\forall 0\le j\lt n$，存在 $0\le h_j\le n$，使得 $A_{i,j}=1\iff i\lt H_j$。

- $\text{Subtask 3 (53 pts)}$：无额外约束。

### 计分方式

如果返回值 `C` 不满足：
- $\forall 0\le i,j\lt n$，都有 $C_{p_i,q_j}=A_{i,j}$ 成立。

那么该测试点得 $0$ 分。

1. 若每组测试数据都有 $k\le 2n-1$，该测试点得满分。
2. 否则，令 $c=\max \{k/n\}$。若 $c\le 10$，得 $(110-9c)/100$ 倍测试点满分。
3. 否则，若 $k\le n^2/2+1$，则得 $7/100$ 倍测试点满分。
4. 否则，该测试点得 $0$ 分。

每个子任务得分为该子任务内测试点得分最小值向下取整。



