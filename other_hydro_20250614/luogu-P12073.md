## 题目描述
There is an array $a$ of length $N$ and an array $b$ of length $M$. All numbers in the arrays are integers and lie in the range from 1 to $k$. There is also an initially empty array $c$.

Alice and Bob play the following game on these arrays: the players take turns, and on their turn, a player must append a number to the end of the array $c$ such that $c$ remains a subsequence of both $a$ and $b$. The player who cannot make a move loses. Alice goes first.

They will play the game $q$ times. For the $i$-th game, they will choose two numbers $x_i$ and $y_i$ ($0 \le x_i < N, 0 \le y_i < M$), then remove the first $x_i$ elements from array $a$ and the first $y_i$ elements from array $b$, and then play the game on the resulting arrays. After each deletion operation and before the next one, the arrays $a$ and $b$ are restored to their initial state, meaning that the numbers deleted from the arrays in one game may not be deleted in subsequent games. Also, the array $c$ is cleared between games.

The guys have their quirks, so they always choose $x_i$ and $y_i$ in such a way that after the deletions, **the remaining parts of arrays $a$ and $b$ start with the same value**.

Alice really wants to win, so she asks you to determine for each game whether she can win, assuming both players play optimally.

Note that the arrays can be very long, so they are provided in a special format. Each array is given as a sequence of segments of equal numbers. Array $a$ consists of $n$ such segments, and array $b$ consists of $m$ such segments. Each segment is defined by its length and the number that occupies that segment.

## 输入格式
The first line contains six integers $N, n, M, m, k, q$ ($1 \le N, M \le 10^9, 1 \le n, m, k \le 1600, 1 \le q \le 10^6$) — the length of the first array, the number of segments in the first array, the length of the second array, the number of segments in the second array, the number limit, and the number of games, respectively.

The next $n$ lines contain two integers $l_i^a$ and $v_i^a$ ($1 \le l_i^a \le N, 1 \le v_i^a \le k$) — the length of the segment and the number written in that segment. These numbers define array $a$: the first $l_1^a$ numbers of array $a$ are equal to $v_1^a$, the next $l_2^a$ numbers are equal to $v_2^a$, ..., the last $l_n^a$ numbers are equal to $v_n^a$.

The next $m$ lines contain two integers $l_i^b$ and $v_i^b$ ($1 \le l_i^b \le N, 1 \le v_i^b \le k$) — the length of the segment and the number written in that segment. These numbers define array $b$. The format is similar to array $a$. It is guaranteed that $\sum l_i^a = N, \sum l_i^b = M, v_i^a \ne v_{i+1}^a$, and $v_i^b \ne v_{i+1}^b$.

The next $q$ lines contain pairs of integers $x_i$ and $y_i$ ($0 \le x_i < N, 0 \le y_i < M$) — descriptions of the games.

For each game $i$, it is guaranteed that if we remove the first $x_i$ elements from $a$ and the first $y_i$ elements from $b$, the remaining parts of the arrays will start with the same value.

## 输出格式
For each of the $q$ games, print "Yes" if Alice wins with optimal strategy, and "No" if Bob wins.

```input1
5 1 5 1 1 9
5 1
5 1
0 0
0 1
0 2
1 0
1 1
1 2
2 0
2 1
2 2
```

```output1
Yes
No
Yes
No
No
Yes
Yes
Yes
Yes
```

```input2
7 3 7 3 2 12
2 1
3 2
2 1
2 2
3 1
2 2
0 2
0 3
0 4
1 2
1 3
1 4
2 5
2 6
3 5
3 6
4 5
4 6
```

```output2
Yes
No
Yes
Yes
No
Yes
No
Yes
No
Yes
Yes
Yes
```

## 提示
**Note**

In the first example, the arrays look like this: $a = (1, 1, 1, 1, 1)$ and $b = (1, 1, 1, 1, 1)$.

*   In the first query, $x = 0, y = 0$, so the game will be played on the arrays $a = (1, 1, 1, 1, 1)$ and $b = (1, 1, 1, 1, 1)$. In this case, players can only append the number 1 to the array $c$, so after 5 moves the game will end, and Bob will lose because he won't be able to make a move.
*   In the second query, $x = 0, y = 1$, so the game will be played on the arrays $a = (1, 1, 1, 1, 1)$ and $b = (1, 1, 1, 1)$. In this case, the game will end after 4 moves, and Alice will lose.
*   In the last query, $x = 2, y = 2$, so the game will be played on the arrays $a = (1, 1, 1)$ and $b = (1, 1, 1)$. In this case, Bob will lose.

In the second example, $a = (1, 1, 2, 2, 2, 1, 1)$, $b = (2, 2, 1, 1, 1, 2, 2)$.

*   In the first query, $x = 0$ and $y = 2$, so the game will be played on the arrays $a = (1, 1, 2, 2, 2, 1, 1)$ and $b = (1, 1, 1, 2, 2)$. If Alice appends the number 2 to the array $c$, Bob will also append the number 2, and then no moves will be left, so Alice will lose. Therefore, Alice must first append the number 1 to $c$. After this, for similar reasons, if Bob appends the number 2 to the array, he will lose. So, he is forced to append the number 1, and the array $c$ becomes $(1, 1)$. Then Alice again appends the number 1 to the array $c$, and Bob has no more moves left, so Alice wins.
*   In the second query, $x = 0$ and $y = 3$, so the game will be played on the arrays $a = (1, 1, 2, 2, 2, 1, 1)$ and $b = (1, 1, 1, 2, 2)$. Following the reasoning in the previous example, Alice cannot append the number 2 to the array $c$, because then she will lose. But if Alice appends the number 1, then Bob will also append the number 1, and after that, Alice will lose for similar reasons. Therefore, Bob wins in this case.

