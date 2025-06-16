## Description

<div><p>An array is called <span class="tex-font-style-it">good</span> if for any element $x$ that appears in this array, it holds that $x$ appears at least twice in this array. For example, the arrays $[1, 2, 1, 1, 2]$, $[3, 3]$, and $[1, 2, 4, 1, 2, 4]$ are good, while the arrays $[1]$, $[1, 2, 1]$, and $[2, 3, 4, 4]$ are not good.</p><p>Milya has two <span class="tex-font-style-bf">good</span> arrays $a$ and $b$ of length $n$. She can rearrange the elements in array $a$ in any way. After that, she obtains an array $c$ of length $n$, where $c_i = a_i + b_i$ ($1 \le i \le n$).</p><p>Determine whether Milya can rearrange the elements in array $a$ such that there are <span class="tex-font-style-bf">at least $3$</span> distinct elements in array $c$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 50$)&nbsp;— the length of the arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the elements of the array $b$.</p></div><div class="output-specification"><p>For each test case, output $«$<span class="tex-font-style-tt">YES</span>$»$ (without quotes) if it is possible to obtain at least $3$ distinct elements in array $c$, and $«$<span class="tex-font-style-tt">NO</span>$»$ otherwise.</p><p>You can output each letter in any case (for example, $«$<span class="tex-font-style-tt">YES</span>$»$, $«$<span class="tex-font-style-tt">Yes</span>$»$, $«$<span class="tex-font-style-tt">yes</span>$»$, $«$<span class="tex-font-style-tt">yEs</span>$»$ will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 50$)&nbsp;— the length of the arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the elements of the array $b$.</p>

## Output

<p>For each test case, output $«$<span class="tex-font-style-tt">YES</span>$»$ (without quotes) if it is possible to obtain at least $3$ distinct elements in array $c$, and $«$<span class="tex-font-style-tt">NO</span>$»$ otherwise.</p><p>You can output each letter in any case (for example, $«$<span class="tex-font-style-tt">YES</span>$»$, $«$<span class="tex-font-style-tt">Yes</span>$»$, $«$<span class="tex-font-style-tt">yes</span>$»$, $«$<span class="tex-font-style-tt">yEs</span>$»$ will be recognized as a positive answer).</p>





```input1|2,3,4,8,9,10,14,15,16
5
4
1 2 1 2
1 2 1 2
6
1 2 3 3 2 1
1 1 1 1 1 1
3
1 1 1
1 1 1
6
1 52 52 3 1 3
59 4 3 59 3 4
4
100 1 100 1
2 2 2 2
```




```output1
YES
YES
NO
YES
NO
```



## Note

<p>In the first test case, you can swap the second and third elements. Then the array $a = [1, 1, 2, 2]$, $b = [1, 2, 1, 2]$, and then $c = [2, 3, 3, 4]$. </p><p>In the second test case, you can leave the elements unchanged. Then $c = [2, 3, 4, 4, 3, 2]$.</p><p>In the third test case, the array $a$ will not change from rearranging the elements in it. Then $c = [2, 2, 2]$, so the answer is $«$<span class="tex-font-style-tt">NO</span>$»$.</p>
