## Description

[NIM](https://en.wikipedia.org/wiki/Nim) is a game of strategy in which two players take turns removing stones from distinct piles. On each turn, a player must remove at least one stone, and may remove any number of stones provided they all come from the same pile. **The player who has no stones to remove loses**.

There are $n$ piles of stones, the $i$-th pile has $l_i$ stones. Alice needs to remove some of the stones from each pile (removing zero or all of the stones from a certain pile is allowed). If the $i$-th pile remains at least one stone after this operation, Alice has to pay a price of $v_i$. After Alice's operation, Bob will create a pile of stones whose number is in $[0,m]$ and add it to the game to make sure that Alice ¡ª the player who moves first in this NIM game will lose. If he can't ensure that Alice will lose, he will exit from the game immediately.  

Now Alice has $q$ queries. Each query gives an integer $c$, and you need to calculate the minimal total price Alice needs to pay to ensure Bob¡¯s new pile has exactly $c$ stones(making Bob exit from the game isn't allowed,even if $c=0$). If this is impossible, print `-1` instead. 

## Input Format

The first line contains two integers $n,m$.  
Each of the following $n$ lines contains two integers $v_i,l_i$.  
The next line contains an integer $q$.
Each of the following $n$ lines contains an integers $c$.  

## Output Format

Output contains $q$ lines,containing the answer of each query in order. Output `-1` if no solution was found.

```input1
4 6
2 3
4 4
3 5
5 2
7
0
1
2
3
4
5
6
```

```output1
0
2
2
2
3
3
5
```

```input2
4 6
2 3
4 4
3 5
5 2
7
0
1
2
3
4
5
6
```

```output2
0
2
2
2
3
3
5
```

## Constraints

For all test cases, $1\le n,q \le 10^5,1\le v_i \le 10^9,0\le l_i\le m\le 10^9,c\in [0,m]$.

Detailed constraints are as follows (blank grids denote the same constraints as mentioned above):

|Subtask #|Score (percentage)|$n,q$|$l_i,m$|Special Constraints|
|:-:|:-:|:-:|:-:|:-:|
|$1$|$15$|$\le 10$|$\le 10$|-|
|$2$|$20$|$\le 100$|$\le 100$|-|
|$3$|$20$|-|-|$\forall i,\exists k\in \mathbb{N}^* \ \text{s.t.}\ l_i=2^k-1$|
|$4$|$20$|$\le 20000$|$\le 20000$|$l_i,v_i$ are randomly generated in range by `std::mt19937` modulo maximum limit|
|$5$|$25$|-|-|$l_i,v_i$ are randomly generated in range by `std::mt19937` modulo maximum limit|

