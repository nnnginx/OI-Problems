## ��Ŀ����
DreamGrid, the king of Gridland, is making a knight tournament. There are $n$ knights, numbered from 1 to $n$, participating in the tournament. The rules of the tournament are listed as follows:

- The tournament consists of $k$ rounds. Each round consists of several duels. Each duel happens between exactly two knights.
- Each knight must participate in exactly one duel during each round.
- For each pair of knights, there can be at most one duel between them during all the $k$ rounds.
- Let $1 \le i, j \le k$, $i \ne j$, and $1 \le a, b, c, d \le n$, $a, b, c, d$ be four distinct integers. If
    - Knight $a$ fights against knight $b$ during round $i$, and
    - Knight $c$ fights against knight $d$ during round $i$, and
    - Knight $a$ fights against knight $c$ during round $j$,
- then knight $b$ must fight against knight $d$ during round $j$.

As DreamGrid's general, you are asked to write a program to arrange all the duels in all the $k$ rounds, so that the resulting arrangement satisfies the rules above. 

## �����ʽ
There are multiple test cases. The first line of the input is an integer $T$, indicating the number of test cases. For each test case:

The first and only line contains two integers $n$ and $k$ ($1 \le n, k \le 1000$), indicating the number of knights participating in the tournament and the number of rounds.

It's guaranteed that neither the sum of $n$ nor the sum of $k$ in all test cases will exceed $5000$.

## �����ʽ
For each test case:

- If it's possible to make a valid arrangement, output $k$ lines. On the $i$-th line, output $n$ integers $c_{i, 1}, c_{i, 2}, \dots, c_{i, n}$ separated by one space, indicating that in the $i$-th round, knight $j$ will fight against knight $c_{i, j}$ for all $1 \le j \le n$.   
If there are multiple valid answers, output the lexicographically smallest answer.   
Consider two answers $A$ and $B$, let's denote $a_{i, j}$ as the $j$-th integer on the $i$-th line in answer $A$, and $b_{i, j}$ as the $j$-th integer on the $i$-th line in answer $B$. Answer $A$ is lexicographically smaller than answer $B$, if there exists two integers $p$ ($1 \le p \le k$) and $q$ ($1 \le q \le n$), such that
    - for all $1 \le i < p$ and $1 \le j \le n$, $a_{i, j} = b_{i, j}$, and
    - for all $1 \le j < q$, $a_{p, j} = b_{p, j}$, and finally $a_{p, q} < b_{p, q}$.
-If it's impossible to make a valid arrangement, output ``Impossible`` (without quotes) in one line.

Please, DO NOT output extra spaces at the end of each line, or your answer may be considered incorrect!

## ��Ŀ����
$n$ ����ʿҪ���� $m$ �ֶԾ���ÿһ��ÿ����ʿ��Ҫ��һ�����֡�����ÿ������ֻ�ܴ�һ�Ρ����� $a$ �� $b$ ���ˣ�$c$ �� $d$ ���ˣ���ô���������һ����� $a$ �� $c$ ���ˣ���ô $b$ �ͱ���� $d$ �����Ƿ���ڷ��������ھ�����ֵ�����С��һ�飬������� ```Impossible```��

```input1
2
3 1
4 3
```

```output1
Impossible
2 1 4 3
3 4 1 2
4 3 2 1
```

