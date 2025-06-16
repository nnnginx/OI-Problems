## Description

<div><p>Given four integers $n$, $m$, $p$, and $q$, determine whether there exists an integer array $a_1, a_2, \ldots, a_n$ (elements may be negative) satisfying the following conditions:</p><ul> <li> The sum of all elements in the array is equal to $m$: $$a_1 + a_2 + \ldots + a_n = m$$ </li><li> The sum of every $p$ consecutive elements is equal to $q$: $$a_i + a_{i + 1} + \ldots + a_{i + p - 1} = q,\qquad\text{ for all }1\le i\le n-p+1$$ </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains four integers $n$, $m$, $p$, and $q$ ($1 \le p \le n \le 100$, $1 \le q, m \le 100$)&nbsp;¡ª the length of the array, the sum of elements, the length of a segment, and the sum of a segment, respectively.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if there exists an array satisfying the above conditions, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will all be recognized as valid responses).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains four integers $n$, $m$, $p$, and $q$ ($1 \le p \le n \le 100$, $1 \le q, m \le 100$)&nbsp;¡ª the length of the array, the sum of elements, the length of a segment, and the sum of a segment, respectively.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if there exists an array satisfying the above conditions, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will all be recognized as valid responses).</p>





```input1|2,4,6
5
3 2 2 1
1 1 1 1
5 4 2 3
10 7 5 2
4 4 1 3
```




```output1
YES
YES
YES
NO
NO
```



## Note

<p>In the first test case, an example of an array satisfying the condition is $[1, 0, 1]$. This is because:</p><ul> <li> $a_1+a_2+a_3 = 1+0+1 = 2 = m$ </li><li> $a_1+a_2=1+0=1=q$ </li><li> $a_2+a_3=0+1=1=q$ </li></ul><p>In the second test case, the only array satisfying the condition is $[1]$.</p><p>In the third test case, an example of an array satisfying the condition is $[-2, 5, -2, 5, -2]$.</p><p>In the fourth test case, it can be proven that there is no array satisfying the condition.</p>
