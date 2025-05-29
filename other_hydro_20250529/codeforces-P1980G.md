## Description

<div><p>Yasya was walking in the forest and accidentally found a tree with $n$ vertices. A tree is a connected undirected graph with no cycles.</p><p>Next to the tree, the girl found an ancient manuscript with $m$ queries written on it. The queries can be of two types.</p><p>The first type of query is described by the integer $y$. The weight of <span class="tex-font-style-bf">each</span> edge in the tree is replaced by the <a href="http://tiny.cc/xor_wiki_eng">bitwise exclusive OR</a> of the weight of that edge and the integer $y$.</p><p>The second type is described by the vertex $v$ and the integer $x$. Yasya chooses a vertex $u$ ($1 \le u \le n$, $u \neq v$) and mentally draws a bidirectional edge of weight $x$ from $v$ to $u$ in the tree.</p><p>Then Yasya finds a simple cycle in the resulting graph and calculates the <a href="http://tiny.cc/xor_wiki_eng">bitwise exclusive OR</a> of all the edges in it. She wants to choose a vertex $u$ such that the calculated value is <span class="tex-font-style-bf">maximum</span>. This calculated value will be the answer to the query. It can be shown that such a cycle exists and is unique under the given constraints (independent of the choice of $u$). If an edge between $v$ and $u$ already existed, a simple cycle is the path $v \to u \to v$.</p><p>Note that the second type of query is performed <span class="tex-font-style-it">mentally</span>, meaning the tree does <span class="tex-font-style-bf">not</span> change in any way after it.</p><p>Help Yasya answer all the queries.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) ！ the number of vertices in the tree and the number of queries.</p><p>The next $n - 1$ lines of each test case contain three integers $v$, $u$, $w$ ($1 \le v, u \le n$, $1 \le w \le 10^9$) ！ the ends of some edge in the tree and its weight.</p><p>It is guaranteed that the given set of edges forms a tree.</p><p>The next $m$ lines of each test case describe the queries: </p><ul> <li> <span class="tex-font-style-tt">^</span> $y$ ($1 \le y \le 10^9$) ！ parameter of the first type query; </li><li> <span class="tex-font-style-tt">?</span> $v$ $x$ ($1 \le v \le n$, $1 \le x \le 10^9$) ！ parameters of the second type query. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. The same is guaranteed for $m$.</p></div><div class="output-specification"><p>For each test case, output the answers to the queries of the second type.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) ！ the number of vertices in the tree and the number of queries.</p><p>The next $n - 1$ lines of each test case contain three integers $v$, $u$, $w$ ($1 \le v, u \le n$, $1 \le w \le 10^9$) ！ the ends of some edge in the tree and its weight.</p><p>It is guaranteed that the given set of edges forms a tree.</p><p>The next $m$ lines of each test case describe the queries: </p><ul> <li> <span class="tex-font-style-tt">^</span> $y$ ($1 \le y \le 10^9$) ！ parameter of the first type query; </li><li> <span class="tex-font-style-tt">?</span> $v$ $x$ ($1 \le v \le n$, $1 \le x \le 10^9$) ！ parameters of the second type query. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. The same is guaranteed for $m$.</p>

## Output

<p>For each test case, output the answers to the queries of the second type.</p>





```input1|2,3,4,5,6,7,8,9,10,11
2
3 7
1 2 1
3 1 8
^ 5
? 2 9
^ 1
? 1 10
^ 6
? 3 1
? 2 9
5 6
1 2 777
3 2 2812
4 1 16
5 3 1000000000
^ 4
? 3 123
? 5 1000000000
^ 1000000000
? 1 908070
? 2 1
```




```input2|2,3,4,5,6,7,8,9,10,11,12,13,25,26,27,28,29,30
3
8 4
8 6 3
6 3 4
2 5 4
7 6 2
7 1 10
4 1 4
5 1 2
^ 4
^ 7
? 7 8
? 4 10
5 6
3 1 4
2 3 9
4 3 6
5 2 10
? 5 7
^ 1
^ 8
? 4 10
? 1 9
? 3 6
4 2
2 1 4
4 3 5
2 3 4
^ 13
? 1 10
```




```output1
13 15 11 10 
1000000127 2812 999756331 999999756
```




```output2
14 13 
13 8 11 11 
10
```


