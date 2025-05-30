## Description

<div><p>Arkady coordinates rounds on some not really famous competitive programming platform. Each round features $n$ problems of distinct difficulty, the difficulties are numbered from $1$ to $n$.</p><p>To hold a round Arkady needs $n$ new (not used previously) problems, one for each difficulty. As for now, Arkady creates all the problems himself, but unfortunately, he can't just create a problem of a desired difficulty. Instead, when he creates a problem, he evaluates its difficulty from $1$ to $n$ and puts it into the problems pool.</p><p>At each moment when Arkady can choose a set of $n$ new problems of distinct difficulties from the pool, he holds a round with these problems and removes them from the pool. Arkady always creates one problem at a time, so if he can hold a round after creating a problem, he immediately does it.</p><p>You are given a sequence of problems' difficulties in the order Arkady created them. For each problem, determine whether Arkady held the round right after creating this problem, or not. Initially the problems pool is empty.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 10^5$)&nbsp;�� the number of difficulty levels and the number of problems Arkady created.</p><p>The second line contains $m$ integers $a_1, a_2, \ldots, a_m$ ($1 \le a_i \le n$)&nbsp;�� the problems' difficulties in the order Arkady created them.</p></div><div class="output-specification"><p>Print a line containing $m$ digits. The $i$-th digit should be $1$ if Arkady held the round after creation of the $i$-th problem, and $0$ otherwise.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 10^5$)&nbsp;�� the number of difficulty levels and the number of problems Arkady created.</p><p>The second line contains $m$ integers $a_1, a_2, \ldots, a_m$ ($1 \le a_i \le n$)&nbsp;�� the problems' difficulties in the order Arkady created them.</p>

## Output

<p>Print a line containing $m$ digits. The $i$-th digit should be $1$ if Arkady held the round after creation of the $i$-th problem, and $0$ otherwise.</p>

## Samples

```input1
3 11
2 3 1 2 2 2 3 2 2 3 1
```

```output1
00100000001
```






```input2
4 8
4 1 3 3 2 3 3 3
```

```output2
00001000
```




## Note

<p>In the first example Arkady held the round after the first three problems, because they are of distinct difficulties, and then only after the last problem.</p>
