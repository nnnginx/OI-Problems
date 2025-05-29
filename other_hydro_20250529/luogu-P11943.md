## 题目背景
版权信息：译自 [2025年度 国际情报 올림피아드 (Olympiad) 代表学生 选拔考试](https://www.ioikorea.or.kr/archives/ioitst/2025/) R1T2。[[CC BY-NC-SA 4.0](http://creativecommons.org/licenses/by-nc-sa/4.0/)]

## 题目描述
本题中，下标默认为 $\textsf{0-index}$。

有一棵 $n$ 个节点的无根树，节点编号 $0\sim {n-1}$。

现在 KOI 研究所开展了粒子碰撞试验。

初始时，每个节点上都没有粒子。

有 $q$ 次操作。每次操作给定 $u,\mathrm{result}$，表示尝试在节点 $u$ 生成一个粒子，生成的结果为 $\mathrm{result}$。

- 若生成成功（$\mathrm{result}=\mathrm{true}$），$u$ 上将存在一个粒子。
- 若生成失败（$\mathrm{result}=\mathrm{false}$），$u$ 将被关闭，无法使用。

我们保证每个节点最多尝试生成 $1$ 次。

一次**碰撞实验**流程如下：选择两个（不同的）节点 $u,v$，满足：
- $u,v$ 上存在粒子；
- $u,v$ 路径上没有其他粒子存在；
- $u,v$ 路径上没有被关闭的节点。

碰撞后，$u,v$ 上的粒子将被销毁。$u,v$ 之后可以出现在其他路径中。

在每次尝试生成后，你需要回答至多能够进行多少次碰撞实验。**注意不会真的进行碰撞实验。**

### 实现细节

你不需要，也不应该实现 `main` 函数。

你应当实现以下的函数：

```cpp
void initialize(int n, std::vector<int> A, std::vector<int> B);
```

`initialize` 函数将在调用 `generate` 前被调用恰好一次。

- $n$：树的节点数量。
- $A,B$：长度为 $(n-1)$ 的数组。$\forall 0\le i\lt n-1$，$A_i,B_i$ 是树上第 $i$ 条边的两个端点。

```cpp
int generate(int u, bool result);
```

表示一次尝试生成粒子的操作。

`generate` 函数将在 `initialize` 函数后调用恰好 $q$ 次。

- $u$：表示尝试在节点 $u$ 生成一个粒子。
- $\mathrm{result}$：生成的结果。
    - 若生成成功（$\mathrm{result}=\mathrm{true}$），$u$ 上将存在一个粒子。
    - 若生成失败（$\mathrm{result}=\mathrm{false}$），$u$ 将被关闭，无法使用。
- 返回一个非负整数，表示在这次尝试后，至多能够进行多少次碰撞实验。

## 输入格式

Sample Grader 输入格式如下：

> $n$ $q$ \
> $A_0$ $B_0$\
> $A_1$ $B_1$\
> $\vdots$\
> $A_{n-2}$ $B_{n-2}$\
> $u_0$ $\mathrm{result}_0$\
> $u_1$ $\mathrm{result}_1$\
> $\vdots$\
> $u_{q-1}$ $\mathrm{result}_{q-1}$

这里，$u_i$ 表示第 $(i-1)$ 次尝试操作对应的节点，$\mathrm{result}_i\in \{\texttt{true},\texttt{false}\}$ 表示生成的结果。

## 输出格式
Sample Grader 输出 $q$ 行，每行一个非负整数，表示答案。


```input1
6
0 1
0 2
0 3
3 4
3 5
1 true
5 true
0 false
4 true
3 true
```

```output1
0
1
0
1
1
```

## 提示

#### 样例交互 $1$

该样例中，$n=6,q=5$，$A=[0,0,0,3,3]$，$B=[1,2,3,4,5]$。树的形态如图所示。

![](https://cdn.luogu.com.cn/upload/image_hosting/wk6cz4kw.png?x-oss-process=image/resize,m_lfit,h_250)

首先交互库调用 
```cpp
initialize(6, [0, 0, 0, 3, 3], [1, 2, 3, 4, 5]);
```

随后调用 

```cpp
generate(1, true);
```

节点 $1$ 上成功生成了一个粒子。最多能够进行 $0$ 次碰撞实验。

![](https://cdn.luogu.com.cn/upload/image_hosting/542wrwnp.png?x-oss-process=image/resize,m_lfit,h_250)

随后调用 

```cpp
generate(5, true);
```

节点 $5$ 上成功生成了一个粒子。最多能够进行 $1$ 次碰撞实验。

![](https://cdn.luogu.com.cn/upload/image_hosting/8hxjbdjd.png?x-oss-process=image/resize,m_lfit,h_250)

随后调用 

```cpp
generate(0, false);
```

节点 $0$ 生成粒子失败，被关闭。由于路径不能经过 $0$，此时最多能够进行 $0$ 次碰撞实验。

![](https://cdn.luogu.com.cn/upload/image_hosting/f7ofp2d4.png?x-oss-process=image/resize,m_lfit,h_250)

随后调用 

```cpp
generate(4, true);
```
节点 $5$ 上成功生成了一个粒子。最多能够进行 $1$ 次碰撞实验。

![](https://cdn.luogu.com.cn/upload/image_hosting/9tqv5jtu.png?x-oss-process=image/resize,m_lfit,h_250)

随后调用 

```cpp
generate(3, true);
```
节点 $3$ 上成功生成了一个粒子。最多能够进行 $1$ 次碰撞实验。

![](https://cdn.luogu.com.cn/upload/image_hosting/1jy0gdpy.png?x-oss-process=image/resize,m_lfit,h_250)


### 数据范围

- $2\le q\le n\le 2\times 10^5$；
- 给定的是一棵树。

### 子任务

- $\text{Subtask 1 (9 pts)}$：$2\le q\le n\le 5\, 000$。
- $\text{Subtask 2 (16 pts)}$：$\forall 0\le i\lt n-1$，$A_i=i,B_i=i+1$。
- $\text{Subtask 3 (20 pts)}$：对于 `generate`，`result=false` 的调用至多有 $20$ 个。
- $\text{Subtask 4 (23 pts)}$：对于 `generate`，`result=true` 的调用至多有 $20$ 个。
- $\text{Subtask 5 (32 pts)}$：无额外约束。

