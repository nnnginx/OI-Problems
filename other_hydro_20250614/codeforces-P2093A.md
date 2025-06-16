## Description

<div><p>We call an array $a$, consisting of $k$ positive integers, palindromic if $[a_1, a_2, \dots, a_k] = [a_k, a_{k-1}, \dots, a_1]$. For example, the arrays $[1, 2, 1]$ and $[5, 1, 1, 5]$ are palindromic, while the arrays $[1, 2, 3]$ and $[21, 12]$ are not.</p><p>We call a number $k$ an ideal generator if any integer $n$ ($n \ge k$) can be represented as the sum of the elements of a palindromic array of length exactly $k$. Each element of the array must be greater than $0$.</p><p>For example, the number $1$ is an ideal generator because any natural number $n$ can be generated using the array $[n]$. However, the number $2$ is not an ideal generator ¡ª there is no palindromic array of length $2$ that sums to $3$.</p><p>Determine whether the given number $k$ is an ideal generator.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) ¡ª the number of test cases.</p><p>The first and only line of each test case contains one integer $k$ ($1 \le k \le 1000$).</p></div><div class="output-specification"><p>For each number $k$, you need to output the word <span class="tex-font-style-tt">"YES"</span> if it is an ideal generator, or <span class="tex-font-style-tt">"NO"</span> otherwise.</p><p>You may output <span class="tex-font-style-tt">"Yes"</span> and <span class="tex-font-style-tt">"No"</span> in any case (for example, the strings <span class="tex-font-style-tt">"yES"</span>, <span class="tex-font-style-tt">"yes"</span>, and <span class="tex-font-style-tt">"Yes"</span> will be recognized as a positive answer).</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$) ¡ª the number of test cases.</p><p>The first and only line of each test case contains one integer $k$ ($1 \le k \le 1000$).</p>

## Output

<p>For each number $k$, you need to output the word <span class="tex-font-style-tt">"YES"</span> if it is an ideal generator, or <span class="tex-font-style-tt">"NO"</span> otherwise.</p><p>You may output <span class="tex-font-style-tt">"Yes"</span> and <span class="tex-font-style-tt">"No"</span> in any case (for example, the strings <span class="tex-font-style-tt">"yES"</span>, <span class="tex-font-style-tt">"yes"</span>, and <span class="tex-font-style-tt">"Yes"</span> will be recognized as a positive answer).</p>





```input1|2,4,6
5
1
2
3
73
1000
```




```output1
YES
NO
YES
YES
NO
```


