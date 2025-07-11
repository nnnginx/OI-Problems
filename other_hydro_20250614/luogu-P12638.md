## 题目描述
Alice and Bob have $n$ piles of stones numbered from $1$ to $n$. In the $i$-th merchant of $a_i$ stones. They perform the following process:

- Alice chooses two non-empty piles. Let there are $x$ and $y$ stones in the piles, respectively.
- Alice takes one stone from each of these piles.
- Next, Bob also chooses two non-empty piles so that they also have $x$ and $y$ stones, respectively. That is, Bob chooses two piles so that they have the same number of stones as was originally in Alice's piles. Bob is allowed to choose the piles that Alice has chosen. If he can't do it, the process ends.
- Bob also takes one stone from his chosen piles.
- If the number of non-empty piles is less than $2$, the described process ends, otherwise it is repeated from the beginning.

Note that Alice does not have to choose the same values of $x$ and $y$ each time.

Alice and Bob want to make sure there are as few stones as possible in the piles. Note that they have a common goal. Help them find the minimum number of stones that may remain.

## 输入格式
The first line contains two integers $n$ and $g$ ($2 \leq n \leq 2 \cdot 10^5$, $0 \leq g \leq 5$) --- the number of piles and the group number.

The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$) --- the number of stones in each pile.

## 输出格式
Print out one integer --- the answer.

```input1
3 0
4 4 3
```

```output1
5
```

```input2
7 0
4 7 7 4 2 2 3
```

```output2
3
```

## 提示
In the first example, Alice can first select the first and third piles: $x=4$ and $y=3$. After she picks up the stones, there will be $3, 4, 2$ stones in the piles, respectively.

Bob has to choose piles with $x=4$ and $y=3$ stones, so he will choose the second and first piles respectively. After he picks up the stones, there will be $2, 3, 2$ stones in the piles, respectively.

In the next step, Alice can choose, for example, the second and third piles: $x=3$ and $y=2$. After she picks up the stones, there will be $2, 2, 1$ stones in the piles, respectively.

Bob will not be able to choose such piles that they have $x=3$ and $y=2$ stones, so the process ends. There are $2+2+1=5$ stones left.

### Scoring

- ($17$ points) $n \le 8$; $a_i \le 8$;
- ($23$ points) $n$ is even; $a_1=a_2,\ a_3=a_4,\ \dots,\ a_{n-1}=a_{n}$;
- ($22$ points) all $a_i$ are even;
- ($18$ points) $a_i \le 2 \cdot 10^5$
- ($20$ points) without additional restrictions.

