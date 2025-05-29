## Description

<div><p>Let's call an array $a$ <span class="tex-font-style-it">beautiful</span> if you can make all its elements the same by using the following operation an arbitrary number of times (possibly, zero): </p><ul> <li> choose an index $i$ ($2 \le i \le |a| - 1$) such that $a_{i - 1} = a_{i + 1}$, and replace $a_i$ with $a_{i - 1}$. </li></ul><p>You are given a beautiful array $a_1, a_2, \dots, a_n$. What is the minimum number of elements you have to remove from it in order for it to stop being beautiful? Swapping elements is prohibited. If it is impossible to do so, then output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>Additional constraints on the input:</p><ul> <li> in every test case, the given array $a$ is beautiful; </li><li> the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$. </li></ul></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of elements you have to remove from the array $a$ in order for it to stop being beautiful. If it is impossible, then output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>Additional constraints on the input:</p><ul> <li> in every test case, the given array $a$ is beautiful; </li><li> the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$. </li></ul>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of elements you have to remove from the array $a$ in order for it to stop being beautiful. If it is impossible, then output <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,3,6,7
4
3
2 2 2
5
1 2 1 2 1
1
1
7
3 3 3 5 3 3 3
```




```output1
-1
1
-1
3
```



## Note

<p>In the first testcase, it is impossible to modify the array in such a way that it stops being beautiful. An array consisting of identical numbers will remain beautiful no matter how many numbers we remove from it.</p><p>In the second testcase, you can remove the number at the index $5$, for example.</p><p>The resulting array will be $[1, 2, 1, 2]$. Let's check if it is beautiful. Two operations are available: </p><ul> <li> Choose $i = 2$: the array becomes $[1, 1, 1, 2]$. No more operations can be applied to it, and the numbers are not all the same. </li><li> Choose $i = 3$ instead: the array becomes $[1, 2, 2, 2]$. No more operations can be applied to it either, and the numbers are still not all the same. </li></ul><p>Thus, the array $[1, 2, 1, 2]$ is not beautiful.</p><p>In the fourth testcase, you can remove the first three elements, for example. The resulting array $[5, 3, 3, 3]$ is not beautiful.</p>
