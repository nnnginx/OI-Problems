## Description

<div><p>One of the first programming problems by K1o0n looked like this: "Noobish_Monk has $n$ $(1 \le n \le 100)$ friends. Each of them gave him $a$ $(1 \le a \le 10000)$ apples for his birthday. Delighted with such a gift, Noobish_Monk returned $b$ $(1 \le b \le \min(10000, a \cdot n))$ apples to his friends. How many apples are left with Noobish_Monk?"</p><p>K1o0n wrote a solution, but accidentally considered the value of $n$ as a string, so the value of $n \cdot a - b$ was calculated differently. Specifically: </p><ul> <li> when multiplying the string $n$ by the integer $a$, he will get the string $s=\underbrace{n + n + \dots + n + n}_{a\ \text{times}}$ </li><li> when subtracting the integer $b$ from the string $s$, the last $b$ characters will be removed from it. If $b$ is greater than or equal to the length of the string $s$, it will become empty. </li></ul><p>Learning about this, ErnKor became interested in how many pairs $(a, b)$ exist for a given $n$, satisfying the constraints of the problem, on which K1o0n's solution gives the correct answer.</p><p>"The solution gives the correct answer" means that it outputs a <span class="tex-font-style-bf">non-empty</span> string, and this string, when converted to an integer, equals the correct answer, i.e., the value of $n \cdot a - b$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$) &nbsp;！ the number of test cases.</p><p>For each test case, a single line of input contains an integer $n$ ($1 \le n \le 100$).</p><p>It is guaranteed that in all test cases, $n$ is distinct.</p></div><div class="output-specification"><p>For each test case, output the answer in the following format:</p><p>In the first line, output the integer $x$&nbsp;！ the number of bad tests for the given $n$.</p><p>In the next $x$ lines, output two integers $a_i$ and $b_i$&nbsp;！ such integers that K1o0n's solution on the test "$n$ $a_i$ $b_i$" gives the correct answer.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$) &nbsp;！ the number of test cases.</p><p>For each test case, a single line of input contains an integer $n$ ($1 \le n \le 100$).</p><p>It is guaranteed that in all test cases, $n$ is distinct.</p>

## Output

<p>For each test case, output the answer in the following format:</p><p>In the first line, output the integer $x$&nbsp;！ the number of bad tests for the given $n$.</p><p>In the next $x$ lines, output two integers $a_i$ and $b_i$&nbsp;！ such integers that K1o0n's solution on the test "$n$ $a_i$ $b_i$" gives the correct answer.</p>





```input1|2,4
3
2
3
10
```




```output1
3
20 18 
219 216 
2218 2214 
1
165 162 
1
1262 2519
```



## Note

<p>In the first example, $a = 20$, $b = 18$ are suitable, as "$\text{2}$" $\cdot 20 - 18 =$ "$\text{22222222222222222222}$"$- 18 = 22 = 2 \cdot 20 - 18$</p>
