## Description

<div><p>Sasha grew up and went to first grade. To celebrate this event her mother bought her a multiplication table $M$ with $n$ rows and $n$ columns such that $M_{ij}=a_i \cdot a_j$ where $a_1, \dots, a_n$ is some sequence of positive integers.</p><p>Of course, the girl decided to take it to school with her. But while she was having lunch, hooligan Grisha erased numbers on the main diagonal and threw away the array $a_1, \dots, a_n$. Help Sasha restore the array!</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \leqslant n \leqslant 10^3$), the size of the table. </p><p>The next $n$ lines contain $n$ integers each. The $j$-th number of the $i$-th line contains the number $M_{ij}$ ($1 \leq M_{ij} \leq 10^9$). The table has zeroes on the main diagonal, that is, $M_{ii}=0$.</p></div><div class="output-specification"><p>In a single line print $n$ integers, the original array $a_1, \dots, a_n$ ($1 \leq a_i \leq 10^9$). It is guaranteed that an answer exists. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($3 \leqslant n \leqslant 10^3$), the size of the table. </p><p>The next $n$ lines contain $n$ integers each. The $j$-th number of the $i$-th line contains the number $M_{ij}$ ($1 \leq M_{ij} \leq 10^9$). The table has zeroes on the main diagonal, that is, $M_{ii}=0$.</p>

## Output

<p>In a single line print $n$ integers, the original array $a_1, \dots, a_n$ ($1 \leq a_i \leq 10^9$). It is guaranteed that an answer exists. If there are multiple answers, print any.</p>

## Samples

```input1
5
0 4 6 2 4
4 0 6 2 4
6 6 0 3 6
2 2 3 0 2
4 4 6 2 0
```

```output1
2 2 3 1 2
```






```input2
3
0 99990000 99970002
99990000 0 99980000
99970002 99980000 0
```

```output2
9999 10000 9998
```



