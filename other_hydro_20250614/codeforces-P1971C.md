## Description

<div><p>There is a clock labeled with the numbers $1$ through $12$ in clockwise order, as shown below.</p><center> <img class="tex-graphics" src="./34654/file/6FYvUpnB.png" style="max-width: 100.0%;max-height: 100.0%;"><p><span class="tex-font-size-small">In this example, $(a,b,c,d)=(2,9,10,6)$, and the strings intersect.</span> </p></center><p>Alice and Bob have four <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$, $d$ not more than $12$. Alice ties a red string connecting $a$ and $b$, and Bob ties a blue string connecting $c$ and $d$. Do the strings intersect? (The strings are straight line segments.)</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 5940$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains four <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$, $d$ ($1 \leq a, b, c, d \leq 12$).</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if the strings intersect, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 5940$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains four <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$, $d$ ($1 \leq a, b, c, d \leq 12$).</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if the strings intersect, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,4,6,8,10,12,14,16
15
2 9 10 6
3 8 9 1
1 2 3 4
5 3 4 12
1 8 2 10
3 12 11 8
9 10 12 1
12 1 10 2
3 12 6 9
1 9 8 4
6 7 9 12
7 12 9 6
10 12 11 1
3 9 6 12
1 4 3 5
```




```output1
YES
NO
NO
YES
YES
NO
NO
NO
NO
NO
NO
YES
YES
YES
YES
```



## Note

<p>The first test case is pictured in the statement.</p><p>In the second test case, the strings do not intersect, as shown below. </p><center> <img class="tex-graphics" src="./34654/file/2Q6Fd197.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
