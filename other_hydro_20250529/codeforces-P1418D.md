## Description

<div><p>Vova decided to clean his room. The room can be represented as the coordinate axis $OX$. There are $n$ piles of trash in the room, coordinate of the $i$-th pile is the integer $p_i$. All piles have <span class="tex-font-style-bf">different</span> coordinates.</p><p>Let's define a <span class="tex-font-style-it">total cleanup</span> as the following process. The goal of this process is to collect <span class="tex-font-style-bf">all</span> the piles in <span class="tex-font-style-bf">no more than two</span> different $x$ coordinates. To achieve this goal, Vova can do several (possibly, zero) moves. During one move, he can choose some $x$ and move <span class="tex-font-style-bf">all piles</span> from $x$ to $x+1$ or $x-1$ using his broom. Note that he can't choose how many piles he will move.</p><p>Also, there are two types of queries:</p><ul> <li> $0$ $x$ �� remove a pile of trash from the coordinate $x$. It is guaranteed that there is a pile in the coordinate $x$ at this moment. </li><li> $1$ $x$ �� add a pile of trash to the coordinate $x$. It is guaranteed that there is no pile in the coordinate $x$ at this moment. </li></ul><p>Note that it is possible that there are zero piles of trash in the room at some moment.</p><p>Vova wants to know the <span class="tex-font-style-bf">minimum</span> number of moves he can spend if he wants to do a <span class="tex-font-style-it">total cleanup</span> before any queries. He also wants to know this number of moves after applying each query. Queries are applied in the given order. Note that the <span class="tex-font-style-it">total cleanup</span> doesn't actually happen and doesn't change the state of piles. It is only used to calculate the number of moves.</p><p>For better understanding, please read the <span class="tex-font-style-bf">Notes</span> section below to see an explanation for the first example.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $q$ ($1 \le n, q \le 10^5$) �� the number of piles in the room before all queries and the number of queries, respectively.</p><p>The second line of the input contains $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le 10^9$), where $p_i$ is the coordinate of the $i$-th pile.</p><p>The next $q$ lines describe queries. The $i$-th query is described with two integers $t_i$ and $x_i$ ($0 \le t_i \le 1; 1 \le x_i \le 10^9$), where $t_i$ is $0$ if you need to remove a pile from the coordinate $x_i$ and is $1$ if you need to add a pile to the coordinate $x_i$. It is guaranteed that for $t_i = 0$ there is such pile in the current set of piles and for $t_i = 1$ there is no such pile in the current set of piles.</p></div><div class="output-specification"><p>Print $q+1$ integers: the minimum number of moves Vova needs to do a <span class="tex-font-style-it">total cleanup</span> before the first query and after each of $q$ queries.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $q$ ($1 \le n, q \le 10^5$) �� the number of piles in the room before all queries and the number of queries, respectively.</p><p>The second line of the input contains $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le 10^9$), where $p_i$ is the coordinate of the $i$-th pile.</p><p>The next $q$ lines describe queries. The $i$-th query is described with two integers $t_i$ and $x_i$ ($0 \le t_i \le 1; 1 \le x_i \le 10^9$), where $t_i$ is $0$ if you need to remove a pile from the coordinate $x_i$ and is $1$ if you need to add a pile to the coordinate $x_i$. It is guaranteed that for $t_i = 0$ there is such pile in the current set of piles and for $t_i = 1$ there is no such pile in the current set of piles.</p>

## Output

<p>Print $q+1$ integers: the minimum number of moves Vova needs to do a <span class="tex-font-style-it">total cleanup</span> before the first query and after each of $q$ queries.</p>

## Samples

```input1
5 6
1 2 6 8 10
1 4
1 9
0 6
0 10
1 100
1 50
```

```output1
5
7
7
5
4
8
49
```






```input2
5 8
5 1 2 4 3
0 1
0 2
0 3
0 4
0 5
1 1000000000
1 1
1 500000000
```

```output2
3
2
1
0
0
0
0
0
499999999
```




## Note

<p>Consider the first example.</p><p>Initially, the set of piles is $[1, 2, 6, 8, 10]$. The answer before the first query is $5$ because you can move all piles from $1$ to $2$ with one move, all piles from $10$ to $8$ with $2$ moves and all piles from $6$ to $8$ with $2$ moves.</p><p>After the first query, the set becomes $[1, 2, 4, 6, 8, 10]$. Then the answer is $7$ because you can move all piles from $6$ to $4$ with $2$ moves, all piles from $4$ to $2$ with $2$ moves, all piles from $2$ to $1$ with $1$ move and all piles from $10$ to $8$ with $2$ moves.</p><p>After the second query, the set of piles becomes $[1, 2, 4, 6, 8, 9, 10]$ and the answer is the same (and the previous sequence of moves can be applied to the current set of piles).</p><p>After the third query, the set of piles becomes $[1, 2, 4, 8, 9, 10]$ and the answer is $5$ because you can move all piles from $1$ to $2$ with $1$ move, all piles from $2$ to $4$ with $2$ moves, all piles from $10$ to $9$ with $1$ move and all piles from $9$ to $8$ with $1$ move.</p><p>After the fourth query, the set becomes $[1, 2, 4, 8, 9]$ and the answer is almost the same (the previous sequence of moves can be applied without moving piles from $10$).</p><p>After the fifth query, the set becomes $[1, 2, 4, 8, 9, 100]$. You can move all piles from $1$ and further to $9$ and keep $100$ at its place. So the answer is $8$.</p><p>After the sixth query, the set becomes $[1, 2, 4, 8, 9, 50, 100]$. The answer is $49$ and can be obtained with almost the same sequence of moves as after the previous query. The only difference is that you need to move all piles from $50$ to $9$ too.</p>
