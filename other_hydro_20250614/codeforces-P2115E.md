## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=wD6_6R7dhnE/">Mayflower by Plum</a></div></div><p>May, Gellyfish's friend, loves playing a game called "Inscryption" which is played on a directed acyclic graph with $n$ vertices and $m$ edges. All edges $ a \rightarrow b$ satisfy $a&lt;b$.</p><p>You start in vertex $1$ with some coins. You need to move from vertex $1$ to the vertex where the boss is located along the directed edges, and then fight with the final boss.</p><p>Each of the $n$ vertices of the graph contains a Trader who will sell you a card with power $w_i$ for $c_i$ coins. You can buy as many cards as you want from each Trader. However, you can only trade with the trader on the $i$-th vertex if you are currently on the $i$-th vertex.</p><p>In order to defeat the boss, you want the sum of the power of your cards to be as large as possible.</p><p>You will have to answer the following $q$ queries:</p><ul> <li> Given integers $p$ and $r$. If the final boss is located at vertex $p$, and you have $r$ coins in the beginning, what is the maximum sum of the power of your cards when you fight the final boss? Note that you are allowed to trade cards on vertex $p$. </li></ul></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $m$ ($1 \leq n \leq 200$, $n - 1 \leq m \leq \min(\frac {n(n-1)} 2, 2000)$)&nbsp;！ the number of vertices and the number of edges.</p><p>The $i$-th of the following $n$ lines of input each contains two integers $c_i$ and $w_i$ ($1 \leq c_i \leq 200$, $1 \leq w_i \leq 10^9$)&nbsp;！ describing the cards of the Trader on the $i$-th vertex.</p><p>In the following $m$ lines of input, each line contains two integers $u$ and $v$ ($1 \leq u &lt; v \leq n$), indicating a directed edge from vertex $u$ to vertex $v$. It is guaranteed that every edge $(u,v)$ appears at most once.</p><p>The next line of input contains one single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>In the following $q$ lines of input, each line contains two integers $p$ and $r$ ($1 \leq p \leq n$, $1 \leq r \leq 10^9$).</p><p>It is guaranteed that for all $i$, there exists a path from vertex $1$ to vertex $i$.</p></div><div class="output-specification"><p>For each query, output the answer to the query.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $m$ ($1 \leq n \leq 200$, $n - 1 \leq m \leq \min(\frac {n(n-1)} 2, 2000)$)&nbsp;！ the number of vertices and the number of edges.</p><p>The $i$-th of the following $n$ lines of input each contains two integers $c_i$ and $w_i$ ($1 \leq c_i \leq 200$, $1 \leq w_i \leq 10^9$)&nbsp;！ describing the cards of the Trader on the $i$-th vertex.</p><p>In the following $m$ lines of input, each line contains two integers $u$ and $v$ ($1 \leq u &lt; v \leq n$), indicating a directed edge from vertex $u$ to vertex $v$. It is guaranteed that every edge $(u,v)$ appears at most once.</p><p>The next line of input contains one single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>In the following $q$ lines of input, each line contains two integers $p$ and $r$ ($1 \leq p \leq n$, $1 \leq r \leq 10^9$).</p><p>It is guaranteed that for all $i$, there exists a path from vertex $1$ to vertex $i$.</p>

## Output

<p>For each query, output the answer to the query.</p>





```input1|
3 2
3 9
2 5
1 2
1 2
2 3
6
1 4
2 4
3 4
1 5
2 5
3 5
```




```input2|
4 4
10 1000
2 5
1 2
3 9
1 2
1 3
2 4
3 4
9
2 3
3 3
4 1
4 2
4 4
4 5
4 101
4 102
4 103
```




```input3|
6 8
9 5
4 1
8 9
10 4
9 4
8 2
3 5
4 6
3 4
2 3
1 2
2 5
4 5
1 3
10
3 12
1 9
6 47
2 19
1 129
5 140
2 148
1 63
2 43
3 102
```




```output1
9
10
11
9
14
14
```




```output2
5
6
2
5
11
14
10002
10005
10009
```




```output3
10
5
46
10
70
154
81
35
21
109
```



## Note

<p>For the third query in the first example, we will play the game in the following order: </p><ul> <li> buy $1$ card with $9$ power from the trader on vertex $1$, and you'll still have $1$ coin after the trade. </li><li> move from vertex $1$ to vertex $2$. </li><li> move from vertex $2$ to vertex $3$. </li><li> buy $1$ card with $2$ power from the trader on vertex $3$, and you'll have no coins after the trade. </li></ul> In the end, we will have $1$ card with $9$ power and $1$ card with $2$, so the sum of the power of the cards is $9+2=11$.<p>For the fifth query in the second example, we will play the game in the following order: </p><ul> <li> move from vertex $1$ to vertex $3$. </li><li> buy $1$ card with $2$ power from the trader on vertex $3$, and you'll still have $3$ coins after the trade. </li><li> move from vertex $3$ to vertex $4$. </li><li> buy $1$ card with $9$ power from the trader on vertex $4$, and you'll have no coins after the trade. </li></ul> In the end, we will have $1$ card with $2$ power and $1$ card with $9$, so the sum of the power of the cards is $2+9=11$.<p>For the sixth query in the second example, we will play the game in the following order: </p><ul> <li> move from vertex $1$ to vertex $2$. </li><li> buy $1$ card with $5$ power from the trader on vertex $2$, and you'll still have $3$ coins after the trade. </li><li> move from vertex $2$ to vertex $4$. </li><li> buy $1$ card with $9$ power from the trader on vertex $4$, and you'll have no coins after the trade. </li></ul> In the end, we will have $1$ card with $5$ power and $1$ card with $9$, so the sum of the power of the cards is $5+9=14$.<p>For the seventh query in the second example, we will play the game in the following order: </p><ul> <li> buy $10$ cards with $1000$ power from the trader on vertex $1$, and you'll still have $1$ coin after the trade. </li><li> move from vertex $1$ to vertex $3$. </li><li> buy $1$ card with $2$ power from the trader on vertex $3$, and you'll have no coins after the trade. </li><li> move from vertex $3$ to vertex $4$. </li></ul> In the end, we will have $10$ cards with $1000$ power and $1$ card with $2$ power, so the sum of the power of the cards is $10 \cdot 1000+2=10\,002$.
