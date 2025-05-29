## Description

Given a sequence  $a_1, a_2, \dots, a_n$, There're $q$ operations you need do execute, divided into two types:

* `1 i x`: Given $i,x$, add $x$ to $a_i$;
* `2 l r`: Given $l,r$, print out $\sum_{i=l}^r a_i$ (i.e. $a_l+a_{l+1}+\dots+a_r$).

## Input

The first line contains 2 integers $n, q$ ¡ª the sequence length and the number of queries. $1\le n,q\le 10^6$.

The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ¡ª the initial sequence. $|a_i|\le 10^6$.

Each of the next $q$ lines contains an operation, `1 i x` or `2 l r`.  
$1\le l\le r\le n, $ $|x|\le 10^6$¡£

## Output

Each line prints the sum $\sum_{i=l}^r a_i$ for an operation 2.

```input1
3 2
1 2 3
1 2 0
2 1 3
```

```output1
6
```

## Limits And Hints

All cases satisfiy $1\le n,q\le 10^6, $ $|a_i|\le 10^6$, $1\le l\le r\le n,$ $|x|\le 10^6$.

