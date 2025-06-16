## Description

<div><p>ErnKor is ready to do anything for Julen, even to swim through crocodile-infested swamps. We decided to test this love. ErnKor will have to swim across a river with a width of $1$ meter and a length of $n$ meters.</p><p>The river is very cold. Therefore, <span class="tex-font-style-bf">in total</span> (that is, throughout the entire swim from $0$ to $n+1$) ErnKor can swim in the water for no more than $k$ meters. For the sake of humanity, we have added not only crocodiles to the river, but also logs on which he can jump. Our test is as follows:</p><p>Initially, ErnKor is on the left bank and needs to reach the right bank. They are located at the $0$ and $n+1$ meters respectively. The river can be represented as $n$ <span class="tex-font-style-it">segments</span>, each with a length of $1$ meter. Each <span class="tex-font-style-it">segment</span> contains either a log <span class="tex-font-style-tt">'L'</span>, a crocodile <span class="tex-font-style-tt">'C'</span>, or just water <span class="tex-font-style-tt">'W'</span>. ErnKor can move as follows: </p><ul> <li> If he is on the surface (i.e., on the bank or on a log), he can jump forward for no more than $m$ ($1 \le m \le 10$) meters (he can jump on the bank, on a log, or in the water). </li><li> If he is in the water, he can only swim to the next river <span class="tex-font-style-it">segment</span> (or to the bank if he is at the $n$-th meter). </li><li> ErnKor cannot land in a <span class="tex-font-style-it">segment</span> with a crocodile in any way. </li></ul><p>Determine if ErnKor can reach the right bank.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains three numbers $n, m, k$ ($0 \le k \le 2 \cdot 10^5$, $1 \le n \le 2 \cdot 10^5$, $1 \le m \le 10$)&nbsp;— the length of the river, the distance ErnKor can jump, and the number of meters ErnKor can swim without freezing.</p><p>The second line of each test case contains a string $a$ of length $n$. $a_i$ denotes the object located at the $i$-th meter. ($a_i \in \{$<span class="tex-font-style-tt">'W'</span>,<span class="tex-font-style-tt">'C'</span>,<span class="tex-font-style-tt">'L'</span>$\}$)</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if ErnKor can pass the test, and output "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains three numbers $n, m, k$ ($0 \le k \le 2 \cdot 10^5$, $1 \le n \le 2 \cdot 10^5$, $1 \le m \le 10$)&nbsp;— the length of the river, the distance ErnKor can jump, and the number of meters ErnKor can swim without freezing.</p><p>The second line of each test case contains a string $a$ of length $n$. $a_i$ denotes the object located at the $i$-th meter. ($a_i \in \{$<span class="tex-font-style-tt">'W'</span>,<span class="tex-font-style-tt">'C'</span>,<span class="tex-font-style-tt">'L'</span>$\}$)</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if ErnKor can pass the test, and output "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11
6
6 2 0
LWLLLW
6 1 1
LWLLLL
6 1 1
LWLLWL
6 2 15
LWLLCC
6 10 0
CCCCCC
6 6 1
WCCCCW
```




```output1
YES
YES
NO
NO
YES
YES
```



## Note

<p>Let's consider examples: </p><ul> <li> First example: We jump from the shore to the first log ($0 \rightarrow 1$), from the first log to the second ($1 \rightarrow 3$), from the second to the fourth ($3 \rightarrow 5$), and from the last log to the shore ($5 \rightarrow 7$). So, we have $0 \rightarrow 1 \rightarrow 3 \rightarrow 5 \rightarrow 7$. Since we did not encounter a crocodile and swam no more than k meters, the answer is <span class="tex-font-style-tt">«YES»</span>. </li><li> Second example: $0 \rightarrow 1$, we jump into the water from the first log ($1 \rightarrow 2$), swim a cell to the log ($2 \leadsto 3$), $3 \rightarrow 4 \rightarrow 5 \rightarrow 6 \rightarrow 7$. Since we did not encounter a crocodile and swam no more than k meters, the answer is <span class="tex-font-style-tt">«YES»</span>. </li><li> In the third example, ErnKor needs to swim two cells <span class="tex-font-style-tt">'W'</span>, but can only swim one. Therefore, the answer is <span class="tex-font-style-tt">«NO»</span>. </li><li> Sixth example: We jump from the shore into the water ($0 \rightarrow 6$) and swim one cell in the water ($6 \leadsto 7$). Since we did not encounter a crocodile and swam no more than k meters, the answer is <span class="tex-font-style-tt">«YES»</span>. </li></ul>
