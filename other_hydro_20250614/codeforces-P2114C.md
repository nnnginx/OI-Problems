## Description

<div><p>Given an array $a$ and $n$ integers. It is sorted in non-decreasing order, that is, $a_i \le a_{i + 1}$ for all $1 \le i &lt; n$.</p><p>You can remove any number of elements from the array (including the option of not removing any at all) without changing the order of the remaining elements. After the removals, the following will occur:</p><ul> <li> $a_1$ is written to a new array;</li><li> if $a_1 + 1 &lt; a_2$, then $a_2$ is written to a new array; otherwise, $a_2$ is written to the same array as $a_1$;</li><li> if $a_2 + 1 &lt; a_3$, then $a_3$ is written to a new array; otherwise, $a_3$ is written to the same array as $a_2$;</li><li> $\cdots$ </li></ul><p>For example, if $a=[1, 2, 4, 6]$, then:</p><ul> <li> $a_1 = 1$ is written to the new array, resulting in arrays: $[1]$; </li><li> $a_1 + 1 = 2$, so $a_2 = 2$ is added to the existing array, resulting in arrays: $[1, 2]$; </li><li> $a_2 + 1 = 3$, so $a_3 = 4$ is written to a new array, resulting in arrays: $[1, 2]$ and $[4]$; </li><li> $a_3 + 1 = 5$, so $a_4 = 6$ is written to a new array, resulting in arrays: $[1, 2]$, $[4]$, and $[6]$. </li></ul><p>Your task is to remove elements in such a way that the described algorithm creates as many arrays as possible. If you remove all elements from the array, no new arrays will be created.</p></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$, $a_i \le a_{i + 1}$) ！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one integer ！ the maximum number of arrays that can be obtained by removing any (possibly zero) number of elements.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$, $a_i \le a_{i + 1}$) ！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output one integer ！ the maximum number of arrays that can be obtained by removing any (possibly zero) number of elements.</p>





```input1|2,3,6,7,10,11
6
6
1 2 3 4 5 6
3
1 2 3
4
1 2 2 4
1
2
3
1 4 8
2
1 1
```




```output1
3
2
2
1
3
1
```



## Note

<p>In the first example, you can remove $a_3$ and $a_5$, then $a=[1, 2, 4, 6]$, the process of forming arrays for it is shown in the statement.</p><p>In the second example, you need to remove $a_2$, after which $a = [1, 3]$, and the arrays $[1]$ and $[3]$ will be written.</p><p>In the third example, no removals are needed; for $a = [1, 2, 2, 4]$, the arrays $[1, 2, 2]$ and $[4]$ will be written.</p>
