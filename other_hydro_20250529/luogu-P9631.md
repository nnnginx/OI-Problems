## ��Ŀ����
Kotori and Umi are playing games of stones, which is hosted by Honoka. The rule is the same as the classic one: There are some piles of stones and the players take turns to remove any positive number of stones from one pile. The one who can't make a legal move loses the game.

This time however, things will be a little different. As the host, Honoka will prepare the games from $n$ candidate piles of stones, where the $i$-th pile initially has $a_i$ stones. Honoka will perform $q$ operations of the following two types:

- Given three integers $l$, $r$ and $x$, for all $l \le i \le r$ change the number of stones in the $i$-th candidate pile to $\max(b_i, x)$, where $b_i$ is the current number of stones in the $i$-th candidate pile.
- Given three integers $l$, $r$ and $x$, start a game of stones consisting of $(r-l+2)$ piles where the $i$-th pile contains $b_{l-1+i}$ stones for all $1 \le i < (r-l+2)$, and the $(r-l+2)$-th pile contains $x$ stones. Note that this operation is only querying for answer and will not affect the state of the $n$ candidate piles of stones.

Kotori is always the first to move. As a big fan of Kotori, you would like to know, for each game of stones, the number of ways Kotori can play in the first step to ensure her victory if both players use the best strategy. We consider two ways different if Kotori is taking stones from different piles, or from the same pile but is taking different number of stones.

## �����ʽ
There is only one test case in each test file.

The first line of the input contains two integers $n$ and $q$ ($1 \le n, q \le 2 \times 10^5$) indicating the number of candidate piles and the number of operations.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($0 \le a_i \le 2^{30}-1$) where $a_i$ indicates the initial number of stones in the $i$-th pile.

For the following $q$ lines, the $i$-th line contains four integers $op_i$, $l_i$, $r_i$ and $x_i$ ($op_i \in \{1, 2\}$, $1 \le l_i \le r_i \le n$, $0 \le x_i \le 2^{30}-1$) indicating the $i$-th operation, where $op_i$ is the type of operation and the others are the parameters of the operation. Operations are given in the order they're performed.

## �����ʽ
For each operation of the second type output one line containing one integer indicating the answer.


## ��Ŀ����
���� $n$ ��ʯ�ѣ��� $i$ ��ʯ�ѵ�ʯ����Ϊ $a_i$���� $q$ �β�����

`1 l r x` ��ʾ���������� $l \leq i \leq r$ �� $a_i$ ��ֵΪ $\max(a_i,x)$��

`2 l r x` ��ʾ��ʯ�� $[l,r]$ ��һ��ʯ����Ϊ $x$ ��ʯ�ѽ��� Nim ��Ϸ�������һ������ȡ��ʯ�Ӻ���Ϸ��Ϊ���ֱذܾ���Ŀɲ����ܷ�������

������㻹���˽� Nim ��Ϸ��[������](https://oi-wiki.org//math/game-theory/impartial-game/)����

���� $100\%$ �����ݱ�֤ $1 \le q,n \le 2 \times 10^5$��$0 \le a_i,x_i \le 2^{30}-1$��$op \in \{1,2\}$��$1 \le l_i,r_i \le n$��

```input1
5 4
1 2 1 4 1
2 1 3 1
1 2 4 3
2 2 4 4
2 1 4 4
```

```output1
1
0
3
```

## ��ʾ
For the first operation the players will play a game of stones consisting of $1$, $2$, $1$ and $1$ stone(s) in each pile respectively. The only winning play for Kotori is reduce the pile with $2$ stones to $1$ stone.

After the second operation, number of stones in the candidate piles changes to $1$, $3$, $3$, $4$ and $1$ respectively.

For the fourth operation the players will play a game of stones consisting of $1$, $3$, $3$, $4$ and $4$ stone(s) in each pile respectively. The winning plays for Kotori is to reduce the pile with $1$ stone to $0$ stone, or to reduce any pile with $3$ stones to $2$ stones.

