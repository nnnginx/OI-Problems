## 题目描述
With the hottest recorded summer ever at Farmer John's farm, he needs a way to cool down his cows. Thus, he decides to invest in some air conditioners.

Farmer John's $N$ cows $(1 \le N \le 20)$ live in a barn that contains a sequence of stalls in a row, numbered $1 \cdots 100$. Cow $i$ occupies a range of these stalls, starting from stall $s_i$ and ending with stall $t_i$. The ranges of stalls occupied by different cows are all disjoint from each-other. Cows have different cooling requirements. Cow $i$ must be cooled by an amount $c_i$, meaning every stall occupied by cow $i$ must have its temperature reduced by at least $c_i$ units.

The barn contains $M$ air conditioners, labeled $1 \cdots M (1 \le M \le 10)$. The $i$-th air conditioner costs $m_i$ units of money to operate $(1 \le m_i \le 1000)$ and cools the range of stalls starting from stall $a_i$ and ending with stall $b_i$. If running, the $i$-th air conditioner reduces the temperature of all the stalls in this range by $p_i (1 \le p_i \le 10^6)$. Ranges of stalls covered by air conditioners may potentially overlap.

Running a farm is no easy business, so FJ has a tight budget. Please determine the minimum amount of money he needs to spend to keep all of his cows comfortable. It is guaranteed that if FJ uses all of his conditioners, then all cows will be comfortable. 

## 输入格式
The first line of input contains $N$ and $M$.

The next $N$ lines describe cows. The ith of these lines contains $s_i, t_i$, and $c_i$.

The next $M$ lines describe air conditioners. The ith of these lines contains $a_i, b_i, p_i$, and $m_i$.

For every input other than the sample, you can assume that $M=10$. 

## 输出格式
Output a single integer telling the minimum amount of money FJ needs to spend to operate enough air conditioners to satisfy all his cows (with the conditions listed above). 

## 题目大意
## 题目描述

农夫约翰的 $N$ 头奶牛 $(1≤N≤20)$ 住在一个谷仓里，谷仓里有连续的牛栏，编号为 $1-100$ 。 奶牛 $i$ 占据了编号 $[s_i,t_i]$ 的牛栏。 不同奶牛占据的牛栏范围是互不相交的。 奶牛有不同的冷却要求，奶牛 $i$ 占用的每个牛栏的温度必须至少降低 $c_i$ 单位。

谷仓包含 $M$ 台空调，标记为 $1-M$ $(1\le M\le10)$。第 $i$ 台空调需要花费 $m_i$ 单位的金钱来运行 $(1\le m_i \le 1000)$ ，如果运行，第 $i$ 台空调将牛栏 $[a_i,b_i]$ 所有牛栏的温度降低 $p_i$（$1\le p_i\le10^6）$。 空调覆盖的牛栏范围可能会重叠。

请帮助农夫约翰求出满足所有奶牛需求要花费的最少金钱。

## 输入格式

第一行两个整数，分别为 $N$ 和 $M$。

第 $2$ 至 $(N+1)$ 行，每行三个整数，分别为 $s_i$、$t_i$ 和 $c_i$ 。

第 $(N+2)$ 至 $(M+N+1)$ 行，每行四个整数， 分别为 $a_i$、$b_i$、$p_i$ 和 $m_i$。

## 输出格式

一个整数，表示最少花费的金钱。



## 提示

### 样例解释 1

一种花费最少的可能解决方案是选择那些冷却区间为 $[2,9]$ 、$[1,2]$ 和 $[6,9]$ 的空调，成本为 $ 3+2+5=10$ .

### 数据范围

对于 $100\%$ 的数据，$1 \le N \le 20$， $1 \le M \le 10$, $ 1 \le a_i, b_i, s_i, t_i \le 100$, $1 \le c_i, p_i \le 10^6$， $1 \le m_i \le 1000$。

```input1
2 4
1 5 2
7 9 3
2 9 2 3
1 6 2 8
1 2 4 2
6 9 1 5
```

```output1
10
```

## 提示
### Explanation for Sample 1

One possible solution that results in the least amount of money spent is to select those that cool the intervals $[2,9], [1,2]$, and $[6,9]$, for a cost of $3+2+5=10$. 

