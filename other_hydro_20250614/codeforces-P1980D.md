## Description

<div><p><span class="tex-font-style-it">GCD</span> (Greatest Common Divisor) of two integers $x$ and $y$ is the maximum integer $z$ by which both $x$ and $y$ are divisible. For example, $GCD(36, 48) = 12$, $GCD(5, 10) = 5$, and $GCD(7,11) = 1$.</p><p>Kristina has an array $a$ consisting of exactly $n$ positive integers. She wants to count the GCD of each neighbouring pair of numbers to get a new array $b$, called <span class="tex-font-style-it">GCD-sequence</span>. </p><p>So, the elements of the GCD-sequence $b$ will be calculated using the formula $b_i = GCD(a_i, a_{i + 1})$ for $1 \le i \le n - 1$.</p><p>Determine whether it is possible to remove <span class="tex-font-style-bf">exactly one</span> number from the array $a$ so that the GCD sequence $b$ is non-decreasing (i.e., $b_i \le b_{i+1}$ is always true).</p><p>For example, let Khristina had an array $a$ = [$20, 6, 12, 3, 48, 36$]. If she removes $a_4 = 3$ from it and counts the GCD-sequence of $b$, she gets:</p><ul> <li> $b_1 = GCD(20, 6) = 2$ </li><li> $b_2 = GCD(6, 12) = 6$ </li><li> $b_3 = GCD(12, 48) = 12$ </li><li> $b_4 = GCD(48, 36) = 12$ </li></ul> The resulting GCD sequence $b$ = [$2,6,12,12$] is non-decreasing because $b_1 \le b_2 \le b_3 \le b_4$.</div><div class="input-specification"><p>The first line of input data contains a single number $t$ ($1 \le t \le 10^4$)&nbsp;！ he number of test cases in the test.</p><p>This is followed by the descriptions of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$) ！ the number of elements in the array $a$.</p><p>The second line of each test case contains exactly $n$ integers $a_i$ ($1 \le a_i \le 10^9$) ！ the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test case does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if you can remove <span class="tex-font-style-bf">exactly one</span> number from the array $a$ so that the GCD-sequence of $b$ is non-decreasing; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will all be recognized as a positive answer).</p></div>

## Input

<p>The first line of input data contains a single number $t$ ($1 \le t \le 10^4$)&nbsp;！ he number of test cases in the test.</p><p>This is followed by the descriptions of the test cases.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2 \cdot 10^5$) ！ the number of elements in the array $a$.</p><p>The second line of each test case contains exactly $n$ integers $a_i$ ($1 \le a_i \le 10^9$) ！ the elements of array $a$.</p><p>It is guaranteed that the sum of $n$ over all test case does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single line: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>" if you can remove <span class="tex-font-style-bf">exactly one</span> number from the array $a$ so that the GCD-sequence of $b$ is non-decreasing; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will all be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11,14,15,18,19,22,23
12
6
20 6 12 3 48 36
4
12 6 3 4
3
10 12 3
5
32 16 8 4 2
5
100 50 2 10 20
4
2 4 8 1
10
7 4 6 2 4 5 1 4 2 8
7
5 9 6 8 5 9 2
6
11 14 8 12 9 3
9
5 7 3 10 6 3 12 6 3
3
4 2 4
8
1 6 11 12 6 12 3 6
```




```output1
YES
NO
YES
NO
YES
YES
NO
YES
YES
YES
YES
YES
```



## Note

<p>The first test case is explained in the problem statement.</p>
