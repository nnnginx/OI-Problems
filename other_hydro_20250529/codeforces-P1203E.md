## Description

<div><p>There are $n$ boxers, the weight of the $i$-th boxer is $a_i$. Each of them can change the weight by no more than $1$ before the competition (the weight cannot become equal to zero, that is, it must remain positive). Weight is always an integer number.</p><p>It is necessary to choose the largest boxing team in terms of the number of people, that all the boxers' weights in the team are different (i.e. unique).</p><p>Write a program that for given current values ​$a_i$ will find the maximum possible number of boxers in a team.</p><p>It is possible that after some change the weight of some boxer is $150001$ (but no more).</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 150000$) — the number of boxers. The next line contains $n$ integers $a_1, a_2, \dots, a_n$, where $a_i$ ($1 \le a_i \le 150000$) is the weight of the $i$-th boxer.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible number of people in a team.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 150000$) — the number of boxers. The next line contains $n$ integers $a_1, a_2, \dots, a_n$, where $a_i$ ($1 \le a_i \le 150000$) is the weight of the $i$-th boxer.</p>

## Output

<p>Print a single integer — the maximum possible number of people in a team.</p>

## Samples

```input1
4
3 2 4 1

```

```output1
4

```






```input2
6
1 1 1 4 4 4

```

```output2
5

```




## Note

<p>In the first example, boxers should not change their weights — you can just make a team out of all of them.</p><p>In the second example, one boxer with a weight of $1$ can be increased by one (get the weight of $2$), one boxer with a weight of $4$ can be reduced by one, and the other can be increased by one (resulting the boxers with a weight of $3$ and $5$, respectively). Thus, you can get a team consisting of boxers with weights of $5, 4, 3, 2, 1$.</p>
