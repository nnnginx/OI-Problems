## Description

<div><p> </p><p>You are given $n^2$ cards with values from $0$ to $n^2-1$. You are to arrange them in a $n$ by $n$ grid such that there is <span class="tex-font-style-bf">exactly</span> one card in each cell.</p><p>The MEX (minimum excluded value) of a subgrid$^{\text{∗}}$ is defined as the smallest non-negative integer that does not appear in the subgrid.</p><p>Your task is to arrange the cards such that the sum of MEX values over all $\left(\frac{n(n+1)}{2}\right)^2$ subgrids is maximized.</p><div class="statement-footnote"><p>$^{\text{∗}}$A subgrid of a $n$ by $n$ grid is specified by four numbers $l_1, r_1, l_2, r_2$ satisfying $1\le l_1\le r_1\le n$ and $1\le l_2\le r_2\le n$. The element in the $i$-th row and the $j$-th column of the grid is part of the subgrid if and only if $l_1\le i\le r_1$ and $l_2\le j\le r_2$.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 500$)&nbsp;— the side length of the grid.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$. </p></div><div class="output-specification"><p>For each test case, output $n$ lines, each containing $n$ integers representing the elements of the grid. </p><p>If there are multiple answers, you can output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 500$)&nbsp;— the side length of the grid.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$. </p>

## Output

<p>For each test case, output $n$ lines, each containing $n$ integers representing the elements of the grid. </p><p>If there are multiple answers, you can output any of them.</p>





```input1|2
2
2
3
```




```output1
0 1 
2 3 
8 4 5 
6 0 1 
7 2 3
```



## Note

<p>In the first test case, one valid arrangement is: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">0</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">1</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td></tr></tbody></table> </center><p>There are $9$ subgrids in total, and the $4$ of them with non-zero MEX are shown below:</p><center><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">0</td></tr></tbody></table> <span class="tex-font-size-small">values:<span class="tex-font-style-it">$[0]$</span>&nbsp;— MEX: <span class="tex-font-style-it">$1$</span></span><p></p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">0</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">1</td></tr></tbody></table> <span class="tex-font-size-small">values:<span class="tex-font-style-it">$[0, 1]$ </span>&nbsp;— MEX: <span class="tex-font-style-it">$2$</span></span><p></p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">0</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td></tr></tbody></table> <span class="tex-font-size-small">values:<span class="tex-font-style-it">$[0, 2]$ </span>&nbsp;— MEX: <span class="tex-font-style-it">$1$</span></span><p></p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">0</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">1</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td></tr></tbody></table> <span class="tex-font-size-small">values:<span class="tex-font-style-it">$[0, 1, 2, 3]$ </span>&nbsp;— MEX: <span class="tex-font-style-it">$4$</span></span><p></p></center><p>The sum of MEX over all subgrids would be $1+2+1+4 = 8$. It can be proven that no other arrangements have a larger sum of MEX values.</p>
