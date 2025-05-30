## 题目描述

> 阿历克斯附体的希尔芬、崩巴附体的切绘、蒸汽姬海老名与全能少女小埋在游乐场玩旋转咖啡杯。双鱼座的切绘占卜得到的幸运数字是 $3$，然而在游乐场却没有编号为 $3$ 的旋转咖啡杯。全能少女小埋想到了办法，旋转咖啡杯的编号构成了一个整数集合，小埋也给出了一个整数集合，并定义了一个操作。现在，她想知道操作后的旋转咖啡杯编号的最低位之和是多少，如果是 $3$，那么她就可以带着切绘去坐旋转咖啡杯啦！

> （以上内容与题目内容无必然联系）

有两个非负整数组成的可重集合 $A$ 和 $B$。

现在你可以对 $A$ 中**至多** $k$ 个元素进行操作。操作方法为：设你准备操作且**未被操作过**的 $A$ 中的元素是 $a$，你可以在 $B$ 中选取任意一个元素 $b$，将 $a$ 修改为 $a\oplus b$（这里 $\oplus$ 表示二进制按位异或），然后从 $B$ 中**删去** $b$。

最终，你要使 $A$ 中所有元素的 $\mathrm{lowbit}$ 之和最小。正整数的 $\mathrm{lowbit}$ 定义为**其二进制最低非零位的值**，$0$ 的 $\mathrm{lowbit}$ 规定为 $0$，例如 $\mathrm{lowbit}(0)=0,\mathrm{lowbit}(1)=1,\mathrm{lowbit}(24)=8$。形式化地有：
$$
\mathrm{lowbit}(x)=
\begin{cases}
\max(\{2^k:k\in \mathbb{N},2^k|x\}) &  x\in \mathbb{N}^+\\
0 & x=0
\end{cases}
$$
（其中 $|$ 表示整除）

你需要求出操作后 $A$ 中所有元素的 $\mathrm{lowbit}$ 之和的可能的最小值。

## 输入格式

第一行一个整数 $n$ 表示 $A$ 的元素个数。  
接下来一行 $n$ 个整数 $\{a_i\}$ 表示 $A$ 中元素。  
接下来一行一个整数 $m$ 表示 $B$ 的元素个数。  
接下来一行 $m$ 个整数 $\{b_i\}$ 表示 $B$ 中元素。  
接下来一行一个整数 $k$。

## 输出格式

输出一行一个整数 $S$ 表示操作后 $A$ 中所有元素的 $\mathrm{lowbit}$ 之和的可能的最小值。

```input1
5
6 18 14 1 13
5
7 7 8 8 15
3
```

```output1
5
```

## 数据范围与提示

对于所有数据，$1\le n,m,k\le 1.2\times 10^6,0\le a_i,b_i\le 10^9$。

|	Subtask #	|	分值		|		$n,m$					|		$k$					|			特殊性质			|
|:-----------------------:|:----------------:|:------------------------------------------------:|:-----------------------------------------:|:------------------------------------------:|
|	1			|	$6$		|	$1\le n,m\le 8$				|	$1\le k\le 8$				|			无				|
|	2			|	$8$		|	$1\le n,m\le 10^6$				|		$k=1$				|	没有元素同时在 $A,B$ 中出现		|
|	3			|	$10$	|	$1\le n,m\le 10^6$				|		$k=1$				|			无				|
|	4			|	$9$		|	$1\le n,m\le 500$				|	$1\le k\le 500$			|	没有元素同时在 $A,B$ 中出现		|
|	5			|	$11$	|	$1\le n,m\le 500$				|	$1\le k\le 500$			|			无				|
|	6			|	$9$		|	$1\le n,m\le 10^6$				|	$1\le k\le 10^6$			|	$B$ 中元素均相等			|
|	7			|	$13$	|	$1\le n,m\le 5\times 10^3$		|	$1\le k\le 5\times 10^3$		|			无				|
|	8			|	$15$	|	$1\le n,m\le 3\times 10^5$		|	$1\le k\le 3\times 10^5$		|			无				|
|	9			|	$19$	|	$1\le n,m\le 1.2\times 10^6$		|	$1\le k\le 1.2\times 10^6$	|			无				|

