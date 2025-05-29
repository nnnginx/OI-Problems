## Description

Moejy0viiiiiv is collecting red envelopes on a rectangular plane. She starts at $(0,0)$. Every day at noon, she walks from $(x, y)$ to $(x,y+1)$ with probability $A/1996488707$, and to $(x+1,y)$ with probability $B/1996488707$, and stops immediately with probability $1-A/1996488707-B/1996488707$ (once she stops, she will never move again). Besides, she also stops after walking for $N$ days. 

With a given constant integer $D$, there¡¯s a red envelope at each $(xD, yD)(0 \leq x, y)$. There¡¯re also $K$ barriers at $(x_1, y_1), (x_2, y_2), (x_3, y_3), ..., (x_K, y_K)$ (barriers never coincide with red envelopes). If she walks to a barrier, she will stop immediately. 

Moejy0viiiiiv will collect each red envelope she passes by (including $(0,0)$). What¡¯s the expected number of red envelopes Moejy0viiiiiv collects after $N$ days? Output the answer $\bmod 998244353$. Notice that $1996488707 \bmod 998244353 = 1$. 

## Input Format

The first line contains two positive integers $A,B$. 

The second line contains four positive integers $N,D,M,K$. 

The following $K$ lines each contains two integers, the $i+2$-th line contains $x_i,y_i$. 

## Output Format

Output contains one integer, the expected number of red envelopes $\bmod 998244353$. 

```input1
1 1
2 2 5 1
1 0
```

```output1
2
```

```input2
1 2
2 2 5 0
```

```output2
6
```

## Constraints 

For all test cases, $1 \leq N \leq 10^{18}, 0 \leq K \leq 50, 1 \leq D, M \leq 1000, 0 \leq x_1, x_2, ..., x_K \leq M$, 
$\forall i \in \{1, 2, 3, ..., K\}, D \nmid x_i \vee D \nmid y_i, x_i + y_i \leq N, 0 \leq A, B < 998244353$. 

Detailed constraints are as follows (blank grids denote the same constraints as mentioned above):

|Subtask #|Score (percentage)|$N$|$D$|$M$|$K$|
|:-:|:-:|:-:|:-:|:-:|:-:|
|$1$|$9$|$\le 10^4$|-|-|-|
|$2$|$12$|$\le 10^5$|$\le 10$|$\le 10$|$0$|
|$3$|$27$|-|-|-|$0$|
|$4$|$8$|$\le 10^5$|$\le  10$|$\le 10$|-|
|$5$|$44$|-|-|-|-|

