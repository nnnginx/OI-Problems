## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/jackblack-sc/peaches">Peaches...</a></span></div><div class="epigraph-source">⠀</div></div><p>Ruby just won an internship position at Farmer John's farm by winning a coding competition! As the newly recruited intern, Ruby is tasked with maintaining Farmer John's peach tree, a tree consisting of $n$ nodes rooted at node $1$. Each node initially contains $a_i = 0$ peaches, and there are two types of events that can happen: </p><ol> <li> Growth event at some node $x$: Ruby must choose <span class="tex-font-style-bf">either</span> the parent of $x$ <span class="tex-font-style-bf">or</span> any node in the subtree of $x$ and increase the amount of peaches it contains by one. </li><li> Harvest event at some node $x$: Ruby must choose a single node that is in the subtree of $x$ and decrease the amount of peaches it contains by one. Note that this is <span class="tex-font-style-bf">not</span> the same set of nodes as the growth event. </li></ol> Note that the subtree of $x$ includes the node $x$ as well.<p>Ruby is also given an array $b$ of length $n$. The peach tree is deemed healthy if $a_i \ge b_i$ for every node $i$.</p><p>Ruby is asked to perform $q$ operations of two types: </p><ul> <li> <span class="tex-font-style-tt">1 x v</span>&nbsp;— Perform $v$ growth events on node $x$. Ruby does <span class="tex-font-style-bf">not</span> have to choose the same node to increase in every growth event. </li><li> <span class="tex-font-style-tt">2 x v</span>&nbsp;— Perform $v$ harvest events on node $x$. Ruby does <span class="tex-font-style-bf">not</span> have to choose the same node to decrease in every harvest event. </li></ul><p>For every prefix of operations, Ruby asks you to find if she can perform these operations <span class="tex-font-style-bf">in some order</span> such that the resulting peach tree (at the end of these operations) is healthy. Note that Ruby can't perform a harvest event that makes any $a_i$ negative.</p><p>Every prefix is independent, meaning that for a given operation, Ruby may choose different nodes to perform events on for every prefix that contains that operation. </p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) &nbsp;— the size of the tree and the number of operations.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1 \le p_i &lt; i$) &nbsp;— the parent of each node.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i \le 10^6$) &nbsp;— the minimum number of peaches each node needs for the peach tree to be considered healthy.</p><p>The next $q$ lines describe the operations Ruby will perform. Each line contains three integers $t$, $x$, and $v$ ($1 \le t \le 2$, $1 \le x \le n$, $1 \le v \le 10^6$). If $t = 1$, this denotes that Ruby must perform $v$ growth events on node $x$. If $t = 2$, this denotes that Ruby must perform $v$ harvest events on node $x$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ and the sum of $q$ does not exceed $2 \cdot 10^5$</p></div><div class="output-specification"><p>For each test case, output $q$ lines. The $i$-th line should contain "<span class="tex-font-style-tt">YES</span>" if Ruby can make the peach tree healthy after performing operations $1, 2, \ldots, i$ in some order. Otherwise, it should contain "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) &nbsp;— the size of the tree and the number of operations.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1 \le p_i &lt; i$) &nbsp;— the parent of each node.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i \le 10^6$) &nbsp;— the minimum number of peaches each node needs for the peach tree to be considered healthy.</p><p>The next $q$ lines describe the operations Ruby will perform. Each line contains three integers $t$, $x$, and $v$ ($1 \le t \le 2$, $1 \le x \le n$, $1 \le v \le 10^6$). If $t = 1$, this denotes that Ruby must perform $v$ growth events on node $x$. If $t = 2$, this denotes that Ruby must perform $v$ harvest events on node $x$.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ and the sum of $q$ does not exceed $2 \cdot 10^5$</p>

## Output

<p>For each test case, output $q$ lines. The $i$-th line should contain "<span class="tex-font-style-tt">YES</span>" if Ruby can make the peach tree healthy after performing operations $1, 2, \ldots, i$ in some order. Otherwise, it should contain "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,5,6,7,8,9,10,11,12
2
8 8
1 1 1 4 3 6 6
5 6 2 9 8 4 1 3
1 3 14
1 4 17
1 2 7
2 2 1
1 6 1
2 1 1000000
1 4 999999
1 3 1
10 20
1 1 1 2 5 2 4 7 2
311353 270334 74853 385085 315501 183346 234819 417314 103862 429437
1 1 837541
1 10 933876
1 1 565958
1 4 791455
2 3 85054
2 3 440978
1 4 981040
1 5 68522
2 1 858305
2 4 184308
1 4 905081
2 8 519626
2 2 269090
1 1 43016
2 2 517644
1 5 355792
1 9 319241
2 10 125447
2 10 523890
1 10 241045
```




```output1
NO
NO
YES
NO
YES
NO
NO
YES
NO
NO
NO
YES
YES
NO
NO
YES
YES
NO
YES
YES
NO
YES
NO
NO
YES
YES
NO
NO
```



## Note

<p>For the prefix containing operations $1, 2, \ldots, 5$ in the first test case, Ruby may perform the operations in the following order:</p><ol> <li> Ruby performs operation $2$ and chooses to increase $a_4$ by $9$ and $a_5$ by $8$. </li><li> Ruby performs operation $1$ and chooses to increase $a_1$ by $5$, $a_3$ by $2$, $a_6$ by $4$, and $a_8$ by $3$. </li><li> Ruby performs operation $3$ and chooses to increase $a_2$ by $7$. </li><li> Ruby performs operation $4$ and chooses to decrease $a_2$ by $1$. </li><li> Ruby performs operation $5$ and chooses to increase $a_7$ by $1$. </li></ol>
