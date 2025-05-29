## Description

<div><p>A beautiful binary matrix is a matrix that has ones on its edges and zeros inside.</p><center> <img class="tex-graphics" src="./34903/file/kGAdUjOQ.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Examples of four beautiful binary matrices.</span> </center><p>Today, Sakurako was playing with a beautiful binary matrix of size $r \times c$ and created a binary string $s$ by writing down all the rows of the matrix, starting from the first and ending with the $r$-th. More formally, the element from the matrix in the $i$-th row and $j$-th column corresponds to the $((i-1)*c+j)$-th element of the string.</p><p>You need to check whether the beautiful matrix from which the string $s$ was obtained could be <span class="tex-font-style-bf">squared</span>. In other words, you need to check whether the string $s$ could have been build from a <span class="tex-font-style-bf">square</span> beautiful binary matrix (i.e., one where $r=c$).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) ！ the length of the string.</p><p>The second line of each test case contains the string $s$ of length $n$. <span class="tex-font-style-bf">The string is always the result of writing out the strings of a beautiful matrix.</span></p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>", if the original matrix could have been square, and "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) ！ the length of the string.</p><p>The second line of each test case contains the string $s$ of length $n$. <span class="tex-font-style-bf">The string is always the result of writing out the strings of a beautiful matrix.</span></p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>", if the original matrix could have been square, and "<span class="tex-font-style-tt">No</span>" otherwise.</p>





```input1|2,3,6,7,10,11
5
2
11
4
1111
9
111101111
9
111111111
12
111110011111
```




```output1
No
Yes
Yes
No
No
```



## Note

<p>For the second test case, string 1111 can be obtained from the matrix:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr></tbody></table> </center><p>For the third test case, string 111101111 can be obtained from the matrix:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr></tbody></table> </center><p>There is no square matrix in the fourth case, such that the string can be obtained from it.</p>
