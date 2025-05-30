## 题目描述
Byteasar is a famous safe-cracker, who renounced his criminal activity and    got into testing and certifying anti-burglary devices.

He has just received a new kind of strongbox for tests: a combinatorial safe.

A combinatorial safe is something different from a combination safe,    even though it is opened with a rotary dial.

The dial can be set in $n$ different positions, numbered from 0 to $n-1$.

Setting the dial in some of these positions opens the safe, while in others it does not.

And here is the combinatorial property, from which the name comes from:

if $x$ and $y$ are opening positions, then so is $(x+y)\ mod\ n$ too;    note that is holds for $x=y$ as well.

Byteasar tried $k$ different positions of the dial: $m_1,m_2,\cdots,m_k$.

The positions $m_1,m_2,\cdots,m_{k-1}$ did not open the safe,only the last position $m_k$ did.

Byteasar is already tired from checking these $k$ positions and has thus    absolutely no intention of trying the remaining ones.

He would like to know however, based on what he already knows about the    positions he tried, what is the maximum possible number of positions that    open the safe.

Help him by writing an appropriate program!

## 输入格式
The first line of the standard input gives two integers $n$ and $k$,      separated by a single space, $1\le k\le 250\ 000$, $k\le n\le 10^{14}$.

The second line holds $k$ different integers, also separated by single      spaces, $m_1,m_2,\cdots,m_k$, $0\le m_i<n$.

You can assume that the input data correspond to a certain combinatorial      safe that complies with the description above.

In tests worth approximately 70% of the points it holds that $k\le 1\ 000$.

In some of those tests, worth approximately 20% of the points,      the following conditions hold in addition: $n\le 10^8$ and $k\le 100$.


## 输出格式
Your program should print out to the first and only line of the standard output a single integer: the maximum number of the dial's positions that can open the safe.


## 题目大意
有一个密码箱，$0$ 到 $n-1$ 中的某些整数是它的密码。且满足：若 $a$ 和 $b$ 是它的密码，则 $(a+b)\bmod n$ 也是它的密码（$a$，$b$ 可以相等）。某人试了 $k$ 次密码，前 $k-1$ 次都失败了，最后一次成功了。

问，该密码箱最多有多少种不同的密码。

## 输入格式

第一行两个整数 $n$，$k$。

第二行为 $k$ 个非负整数，表示每次试的密码。

## 输出格式

一行一个整数，表示答案。

```input1
42 5
28 31 10 38 24
```

```output1
14
```

