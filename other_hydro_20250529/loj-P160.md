## Description

There're $N$ items numbered from $1\ldots N$, each item $i$ with a weight $w_i$ and a value $v_i$. The knapsack's capacity is $W$.

Some items could be selected only after a specific item have been put into the knapsack, or in other words, 
 some items depend on others.  
+ $d_i = j$ $(i>j>0)$ means item $i$ depends on item $j$, you cannot choose item $i$ until you put item $j$ into the knapsack.  
+ $d_i = 0$ $(i>0)$ means item $i$ does not depends on any other items. 

It's guaranteed that each item depends on no more than one item. All the dependency relationships are vaild, no loop.

Maximize the sum of the values of the items in the knapsack so that the sum of the weights is no more than the knapsack's capacity.

## Input

$N\ \ W$  
$d_{\large 1\dots N}$  
$w_{\large 1\dots N}$  
$v_{\large 1\dots N}$

## Output

A single integer, represents your answer.

```input4
7 0
3 4 5 3 0 7 0
1 2 2 1 1 2 2
1 1 2 3 1 1 2
```

```output4
0
```

```input1
7 4
3 4 5 3 0 7 0
1 2 2 1 1 2 2
1 1 2 3 1 1 2
```

```output1
6
```

```input2
10 6
0 1 1 1 2 3 4 5 6 7
1 1 2 2 3 1 2 2 3 1
0 1 1 1 1 1 1 1 1 1
```

```output2
3
```

```input3
13 3
0 1 1 1 3 3 0 0 8 9 10 8 10
1 1 1 1 1 1 1 1 1 1 1 1 1
2 16 32 512 2048 4096 4 1 8 64 1024 128 256
```

```output3
4130
```

```input4
13 25
0 1 1 1 3 3 0 0 8 9 10 8 10
5 6 4 3 7 5 4 7 3 6 5 6 6
0 2 1 2 3 3 3 0 1 2 4 3 2
```

```output4
10
```

## Limits And Hints

$1\le N¡ÁW\le 6¡Á10^7,$ $1\le N\le 5¡Á10^4,$ $0\le W\le 6¡Á10^4;$

$1\le w_i\le 200;$

$0\le v_i\le 5000$.

|Subtask id|pts |$N=$  |$W\le$   |Additional Constraints        |Dependencies |
|:--:|:-:|:---:|:----:|:--------:|:-----:|
| 1  | &#8203;1  | 21  |  25  | Bare-root Forest  |       |
| 2  | &#8203;2  | 22  |  26  |   A Single Tree    |       |
| 3  | &#8203;3  | 23  |  27  |    Flower    |       |
| 4  | &#8203;4  | 24  |  28  |    A Forest    |   2   |
| 5  | &#8203;5  | 100 | 120  |   A Single Tree    |1, 3, 4|
| 6  | &#8203;10 | 200 | 250  |Forest£¬$v_i=1$|   5   |
| 7  | 10 | 200 | 200  |Forest£¬$w_i=1$|   5   |
| 8  | &#8203;10 | 200 | 250  |    &#8203;Forest    |  6, 7  |
| 9  |15 | 400 | 500  |    &#8203;Forest    |   8   |
| 10 | &#8203;20 |7500 | 8000 |    Forest    |   9   |
| 11 | 10 |50000| 1200 |    Forest    |  10   |
| 12 | &#8203;10 |1000 |60000 |    Forest    |  10   |

