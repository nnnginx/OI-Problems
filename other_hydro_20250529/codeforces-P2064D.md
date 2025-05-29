## Description

<div><p>There are $n$ slimes on a line, the $i$-th of which has weight $w_i$. Slime $i$ is able to eat another slime $j$ if $w_i \geq w_j$; afterwards, slime $j$ disappears and the weight of slime $i$ becomes $w_i \oplus w_j$$^{\text{∗}}$.</p><p>The King of Slimes wants to run an <span class="tex-font-style-it">experiment with parameter</span> $x$ as follows: </p><ul> <li> Add a new slime with weight $x$ to the right end of the line (after the $n$-th slime). </li><li> This new slime eats the slime to its left if it is able to, and then takes its place (moves one place to the left). It will continue to do this until there is either no slime to its left or the weight of the slime to its left is greater than its own weight. (No other slimes are eaten during this process.) </li><li> The <span class="tex-font-style-it">score</span> of this experiment is the total number of slimes eaten. </li></ul><p>The King of Slimes is going to ask you $q$ queries. In each query, you will be given an integer $x$, and you need to determine the score of the experiment with parameter $x$.</p><p>Note that the King does not want you to actually perform each experiment; his slimes would die, which is not ideal. He is only asking what the hypothetical score is; in other words, the queries are <span class="tex-font-style-bf">not</span> persistent.</p><div class="statement-footnote"><p>$^{\text{∗}}$Here $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p></div></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the number of slimes and the number of queries, respectively.</p><p>The following line contains $n$ integers $w_1,w_2,\ldots,w_n$ ($1 \le w_i &lt; 2^{30}$)&nbsp;— the weights of the slimes.</p><p>The following $q$ lines contain a single integer $x$ ($ 1 \le x &lt; 2^{30}$)&nbsp;— the parameter for the experiment.</p><p>The sum of $n$ does not exceed $2 \cdot 10^5$ and the sum of $q$ does not exceed $2 \cdot 10^5$ across all test cases.</p></div><div class="output-specification"><p>For each query, output a single integer&nbsp;— the score of the experiment.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;— the number of slimes and the number of queries, respectively.</p><p>The following line contains $n$ integers $w_1,w_2,\ldots,w_n$ ($1 \le w_i &lt; 2^{30}$)&nbsp;— the weights of the slimes.</p><p>The following $q$ lines contain a single integer $x$ ($ 1 \le x &lt; 2^{30}$)&nbsp;— the parameter for the experiment.</p><p>The sum of $n$ does not exceed $2 \cdot 10^5$ and the sum of $q$ does not exceed $2 \cdot 10^5$ across all test cases.</p>

## Output

<p>For each query, output a single integer&nbsp;— the score of the experiment.</p>





```input1|2,3,4,11,12,13,14,15,16,17,18,19,20,21
3
1 1
5
6
4 4
1 5 4 11
8
13
16
15
10 9
10 4 3 9 7 4 6 1 9 4
2
6
5
6
9
8
6
2
7
```




```output1
1
0 2 4 2
0 1 1 1 3 3 1 0 1
```



## Note

<p>For the first query of the <span class="tex-font-style-it">second</span> testcase: </p><ul> <li> A slime of weight $8$ would be added to the end, so $w = [1, 5, 4, 11, \color{red}8]$. </li><li> The added slime has smaller weight than the slime to its left so it cannot eat it, and thus ends the process after eating no slimes with score $0$. </li></ul> For the second query of the second testcase: <ul> <li> A slime of weight $13$ would be added to the end, so $w = [1, 5, 4, 11, \color{red}{13}]$. </li><li> The added slime has bigger weight than the slime to its left, and so it will eat it. Its weight will become $13 \oplus 11 = 6$. Now $w = [1, 5, 4, \color{red}{6}]$. </li><li> The added slime will now eat the slime to its left, and its weight becomes $6 \oplus 4 = 2$. Now $w = [1, 5, \color{red}{2}]$. </li><li> The added slime is no longer able to eat the slime to its left, so it ends the process with a score of $2$. </li></ul>
