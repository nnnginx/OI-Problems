## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">MOOOOOOOOOOOOOOOOO</span></div><div class="epigraph-source">〞 Bessie the Cow, <span class="tex-font-style-it">The Art of Racing on Islands</span></div></div><p>Two of Farmer John's cows, Bessie and Elsie, are planning to race on $n$ islands. There are $n - 1$ <span class="tex-font-style-it">main</span> bridges, connecting island $i$ to island $i + 1$ for all $1 \leq i \leq n - 1$. Additionally, there are $m$ alternative bridges. Elsie can use <span class="tex-font-style-bf">both</span> main and alternative bridges, while Bessie can only use main bridges. All bridges are <span class="tex-font-style-bf">one way</span> and can only be used to travel from an island with a lower index to an island with a higher index.</p><p>Initially, Elsie starts on island $1$, and Bessie starts on island $s$. The cows alternate turns, with Bessie making the first turn. Suppose the cow is on island $i$. During a cow's turn, if there are any bridges connecting island $i$ to island $j$, then the cow can move to island $j$. Then, island $i$ collapses, and all bridges connecting to island $i$ also collapse. Also, note the following:</p><ul> <li> If there are no bridges connecting island $i$ to another island, then island $i$ collapses, and this cow is eliminated from the race. </li><li> If the other cow is also on island $i$, then after this cow moves to another island, the island collapses, and the other cow is eliminated from the race. </li><li> After an island or bridge collapses, no cows may use them. </li><li> If a cow is eliminated, their turn is skipped for the rest of the race. </li></ul><p>The race ends once either cow reaches island $n$. It can be shown that regardless of the cows' strategies, at least one cow reaches island $n$. Bessie wins if and only if she reaches island $n$ first.</p><p>For each $1 \leq s \leq n - 1$, determine whether Bessie wins if she starts the race on island $s$. Assume both cows follow optimal strategies to ensure their own respective victories.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;每 the number of test cases.</p><p>The first line of each test case contains $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^5$, $0 \leq m \leq 2 \cdot 10^5$)&nbsp;每 the number of islands and the number of alternative bridges.</p><p>The next $m$ lines of each test case contain $u$ and $v$ ($1 \leq u &lt; v \leq n$)&nbsp;每 the islands that the alternative bridge connects. It is guaranteed all alternative bridges are distinct, and they do not coincide with the main bridges.</p><p>It is guaranteed that neither the sum of $n$ nor the sum of $m$ over all test cases exceeds $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a binary string of length $n - 1$ on a new line. The $i$'th character is $1$ if it is possible for Bessie to win if she starts on island $i$. Otherwise, it is $0$.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;每 the number of test cases.</p><p>The first line of each test case contains $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^5$, $0 \leq m \leq 2 \cdot 10^5$)&nbsp;每 the number of islands and the number of alternative bridges.</p><p>The next $m$ lines of each test case contain $u$ and $v$ ($1 \leq u &lt; v \leq n$)&nbsp;每 the islands that the alternative bridge connects. It is guaranteed all alternative bridges are distinct, and they do not coincide with the main bridges.</p><p>It is guaranteed that neither the sum of $n$ nor the sum of $m$ over all test cases exceeds $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a binary string of length $n - 1$ on a new line. The $i$'th character is $1$ if it is possible for Bessie to win if she starts on island $i$. Otherwise, it is $0$.</p>





```input1|2,5,6,12,13,14,15
5
6 0
6 1
2 6
6 1
1 5
10 4
1 3
1 6
2 7
3 8
15 3
2 8
4 9
8 15
```




```output1
11111
11011
10011
100001111
11000111000111
```



## Note

<p>In the first test case, there are no alternative bridges for Elsie to overtake Bessie and reach island $n$ first, so Bessie will win on all islands because she always moves first.</p><p>In the second case, Bessie will lose if she starts on island $3$ because:</p><ul> <li> Bessie's Turn: Take a main bridge from island $3$ to island $4$. </li><li> Elsie's Turn: Take a main bridge from island $1$ to island $2$. </li><li> Bessie's Turn: Take a main bridge from island $4$ to island $5$. </li><li> Elsie's Turn: Take an alternative bridge from island $2$ to island $6$. Elsie reaches island $n$ first. </li></ul>
