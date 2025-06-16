## Description

<div><p>The cost of a positive integer $n$ is defined as the result of dividing the number $n$ by the sum of its digits.</p><p>For example, the cost of the number $104$ is $\frac{104}{1 + 0 + 4} = 20.8$, and the cost of the number $111$ is $\frac{111}{1 + 1 + 1} = 37$.</p><p>You are given a positive integer $n$ that does not contain leading zeros. You can remove any number of digits from the number $n$ (including none) so that the remaining number contains at least one digit and <span class="tex-font-style-bf">is strictly greater than zero</span>. The remaining digits <span class="tex-font-style-bf">cannot</span> be rearranged. As a result, you <span class="tex-font-style-bf">may</span> end up with a number that has leading zeros.</p><p>For example, you are given the number $103554$. If you decide to remove the digits $1$, $4$, and one digit $5$, you will end up with the number $035$, whose cost is $\frac{035}{0 + 3 + 5} = 4.375$.</p><p>What is the minimum number of digits you need to remove from the number so that its cost becomes the minimum possible?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$) ！ the number of test cases.</p><p>The only line of each test case contains a positive integer $n$ ($1 \leq n &lt; 10^{100}$) without leading zeros.</p></div><div class="output-specification"><p>For each test case, output one integer on a new line ！ the number of digits that need to be removed from the number so that its cost becomes minimal.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$) ！ the number of test cases.</p><p>The only line of each test case contains a positive integer $n$ ($1 \leq n &lt; 10^{100}$) without leading zeros.</p>

## Output

<p>For each test case, output one integer on a new line ！ the number of digits that need to be removed from the number so that its cost becomes minimal.</p>





```input1|2,4
4
666
13700
102030
7
```




```output1
2
4
3
0
```


