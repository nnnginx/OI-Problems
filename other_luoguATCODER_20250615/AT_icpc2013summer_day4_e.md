# AT_icpc2013summer_day4_e Optimal alpha beta pruning

## 题目描述

$ \color{red} \text{Sorry, problem statement was modified.(12:51 JST)}$

Fox Ciel is developing an artificial intelligence (AI) for a game. This game is described as a game tree T with n vertices. Each node in the game has an evaluation value which shows how good a situation is. This value is the same as maximum value of child nodes' values multiplied by -1. Values on leaf nodes are evaluated with Ciel's special function -- which is a bit heavy. So, she will use alpha-beta pruning for getting root node's evaluation value to decrease the number of leaf nodes to be calculated.

By the way, changing evaluation order of child nodes affects the number of calculation on the leaf nodes. Therefore, Ciel wants to know the minimum and maximum number of times to calculate in leaf nodes when she could evaluate child node in arbitrary order. She asked you to calculate minimum evaluation number of times and maximum evaluation number of times in leaf nodes.

$\color{red}\text{Added pseudocode.(13:17 JST)}$

Ciel uses following algotithm:

```
function negamax(node, α, β)
    if node is a terminal node
        return value of leaf node
    else
        foreach child of node
            val := -negamax(child, -β, -α)
            if val >= β
                return val
            if val > α
                α := val
        return α
```

\[NOTE\] [negamax algorithm](http://en.wikipedia.org/wiki/Negamax)

## 输入格式

Input follows following format:

> $n$  
> $p_1 p_2 \dots p_n$  
> $k_1 t_{11} t_{12} \dots t_{1k}$  
> $\vdots$  
> $\vdots$  
> $k_n t_{n1} t_{n2} \dots t_{nk}$

The first line contains an integer $n$, which means the number of vertices in game tree T.

The second line contains $n$ integers $p_i$, which means the evaluation value of vertex $i$.

Then, next $n$ lines which contain the information of game tree T.

$k_i$ is the number of child nodes of vertex $i$, and $t_{ij}$ is the indices of the child node of vertex $i$.

Input follows following constraints:

- $2 \le n \le 100$
- $-10,000 \le p_i \le 10,000$
- $0 \le k_i \le 5$
- $2 \le t_{ij} \le n$
- Index of root node is $1$.
- Evaluation value except leaf node is always $0$. This does not mean the evaluation values of non-leaf nodes are 0. You have to calculate them if necessary.
- Leaf node sometimes have evaluation value of $0$.
- Game tree T is tree structure.

## 输出格式

Print the minimum evaluation number of times and the maximum evaluation number of times in leaf node.

Please separated by whitespace between minimum and maximum.

```plaintext
minimum maximum
```

## 说明/提示

Source Name\: [Summer Camp 2013](http://acm-icpc.aitea.net/index.php?2013%2FPractice%2F%B2%C6%B9%E7%BD%C9).