## Description

<div><p>You have a strip of paper with a binary string $s$ of length $n$. You can fold the paper in between any pair of adjacent digits.</p><p>A set of folds is considered <span class="tex-font-style-it">valid</span> if after the folds, all characters that are on top of or below each other match. Note that all folds are made at the same time, so the characters don't have to match in between folds.</p><p>For example, these are valid foldings of $s = \mathtt{110110110011}$ and $s = \mathtt{01110}$:</p><center> <img class="tex-graphics" src="./34603/file/Ntf9xKOk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The length of the folded strip is the length seen from above after all folds are made. So for the two above examples, after the folds shown above, the lengths would be $7$ and $3$, respectively.</p><p>Notice that for the above folding of $s = \mathtt{01110}$, if we made either of the two folds on their own, that would not be a valid folding. However, because we don't check for validity until all folds are made, this folding is valid.</p><p>After performing a set of valid folds, what is the minimum length strip you can form?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2\cdot 10^5$)&nbsp;！ the size of the strip.</p><p>The second line of each test case contains a string $s$ of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'&nbsp;！ a description of the digits on the strip.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum possible length of the strip after a valid folding.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2\cdot 10^5$)&nbsp;！ the size of the strip.</p><p>The second line of each test case contains a string $s$ of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'&nbsp;！ a description of the digits on the strip.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum possible length of the strip after a valid folding.</p>





```input1|2,3,6,7,10,11
6
6
101101
1
0
12
110110110011
5
01110
4
1111
2
01
```




```output1
3
1
3
3
1
2
```



## Note

<p>For the first example case, one optimal folding is to fold the strip in the middle, which produces a strip of length 3.</p><p>The third and fourth example cases correspond to the images above. Note that the folding shown above for $s = \mathtt{110110110011}$ is not of minimal length.</p>
