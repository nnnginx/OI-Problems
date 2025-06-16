## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. In this version, $n=m$ and the time limit is lower. You can make hacks only if both versions of the problem are solved.</span></p><p>In the court of the Blue King, Lelle and Flamm are having a performance match. The match consists of several rounds. In each round, either Lelle or Flamm wins.</p><p>Let $W_L$ and $W_F$ denote the number of wins of Lelle and Flamm, respectively. The Blue King considers a match to be <span class="tex-font-style-bf">successful</span> if and only if:</p><ul> <li> after every round, $\gcd(W_L,W_F)\le 1$; </li><li> at the end of the match, $W_L\le n, W_F\le m$. </li></ul><p>Note that $\gcd(0,x)=\gcd(x,0)=x$ for every non-negative integer $x$.</p><p>Lelle and Flamm can decide to stop the match whenever they want, and the final score of the performance is $l \cdot W_L + f \cdot W_F$.</p><p>Please help Lelle and Flamm coordinate their wins and losses such that the performance is <span class="tex-font-style-bf">successful</span>, and the total score of the performance is maximized.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1\leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains four integers $n$, $m$, $l$, $f$ ($2\leq n\leq m \leq 2\cdot 10^7$, $1\leq l,f \leq 10^9$, $\bf{n=m}$): $n$, $m$ gives the upper bound on the number of Lelle and Flamm's wins, $l$ and $f$ determine the final score of the performance.</p><p><span class="tex-font-style-bf">Unusual additional constraint</span>: it is guaranteed that, for each test, there are no pairs of test cases with the same pair of $n$, $m$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the maximum total score of a <span class="tex-font-style-bf">successful</span> performance.</p></div>

## Input

<p>The first line contains an integer $t$ ($1\leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains four integers $n$, $m$, $l$, $f$ ($2\leq n\leq m \leq 2\cdot 10^7$, $1\leq l,f \leq 10^9$, $\bf{n=m}$): $n$, $m$ gives the upper bound on the number of Lelle and Flamm's wins, $l$ and $f$ determine the final score of the performance.</p><p><span class="tex-font-style-bf">Unusual additional constraint</span>: it is guaranteed that, for each test, there are no pairs of test cases with the same pair of $n$, $m$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the maximum total score of a <span class="tex-font-style-bf">successful</span> performance.</p>





```input1|2,4,6,8
8
3 3 2 5
4 4 1 4
6 6 2 2
7 7 2 3
9 9 9 1
2 2 1 4
5 5 1 4
8 8 6 7
```




```input2|2
1
20000000 20000000 1341 331
```




```input3|2
2
1984 1984 19 84
9982 9982 44 35
```




```output1
19
17
18
33
86
9
24
86
```




```output2
33439999007
```




```output3
204143
788403
```



## Note

<p>In the first test case, a possible performance is as follows:</p><ul> <li> Flamm wins, $\gcd(0,1)=1$. </li><li> Lelle wins, $\gcd(1,1)=1$. </li><li> Flamm wins, $\gcd(1,2)=1$. </li><li> Flamm wins, $\gcd(1,3)=1$. </li><li> Lelle wins, $\gcd(2,3)=1$. </li><li> Lelle and Flamm agree to stop the match. </li></ul><p>The final score is $2\cdot2+3\cdot5=19$.</p><p>In the third test case, a possible performance is as follows:</p><ul> <li> Flamm wins, $\gcd(0,1)=1$. </li><li> Lelle wins, $\gcd(1,1)=1$. </li><li> Lelle wins, $\gcd(2,1)=1$. </li><li> Lelle wins, $\gcd(3,1)=1$. </li><li> Lelle wins, $\gcd(4,1)=1$. </li><li> Lelle wins, $\gcd(5,1)=1$. </li><li> Flamm wins, $\gcd(5,2)=1$. </li><li> Flamm wins, $\gcd(5,3)=1$. </li><li> Flamm wins, $\gcd(5,4)=1$. </li><li> Lelle and Flamm agree to stop the match. </li></ul><p>The final score is $5\cdot2+4\cdot2=18$. Note that Lelle and Flamm can stop the match even if neither of them has $n$ wins.</p>
