## Description

<div><p>Due to a shortage of teachers in the senior class of the "T-generation", it was decided to have a huge male gorilla conduct exams for the students. However, it is not that simple; to prove his competence, he needs to solve the following problem.</p><p>For an array $b$, we define the function $f(b)$ as the smallest number of the following operations required to make the array $b$ empty: </p><ul> <li> take two integers $l$ and $r$, such that $l \le r$, and let $x$ be the $\min(b_l, b_{l+1}, \ldots, b_r)$; then </li><li> remove all such $b_i$ that $l \le i \le r$ and $b_i = x$ from the array, the deleted elements are removed, the indices are renumerated. </li></ul><p>You are given an array $a$ of length $n$ and an integer $k$. No more than $k$ times, you can choose any index $i$ ($1 \le i \le n$) and any integer $p$, and replace $a_i$ with $p$.</p><p>Help the gorilla to determine the smallest value of $f(a)$ that can be achieved after such replacements.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each set of input data contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $0 \le k \le n$)&nbsp;！ the length of the array $a$ and the maximum number of changes, respectively.</p><p>The second line of each set of input data contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the array $a$ itself.</p><p>It is guaranteed that the sum of the values of $n$ across all sets of input data does not exceed $10^5$.</p></div><div class="output-specification"><p>For each set of input data, output a single integer on a separate line&nbsp;！ the smallest possible value of $f(a)$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each set of input data contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $0 \le k \le n$)&nbsp;！ the length of the array $a$ and the maximum number of changes, respectively.</p><p>The second line of each set of input data contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the array $a$ itself.</p><p>It is guaranteed that the sum of the values of $n$ across all sets of input data does not exceed $10^5$.</p>

## Output

<p>For each set of input data, output a single integer on a separate line&nbsp;！ the smallest possible value of $f(a)$.</p>





```input1|2,3,6,7,10,11
6
1 0
48843
3 1
2 3 2
5 3
1 2 3 4 5
7 0
4 7 1 3 2 4 1
11 4
3 2 1 4 4 3 4 2 1 3 3
5 5
1 2 3 4 5
```




```output1
1
1
2
5
2
1
```



## Note

<p>In the first set of input data, $f([48\,843]) = 1$, since the array consists of a single number, and thus it can be removed in one operation.</p><p>In the second set of input data, you can change the second number to $2$, resulting in the array $[2, 2, 2]$, where $f([2, 2, 2]) = 1$, since you can take the entire array as a subarray, the minimum on it is $2$, so we will remove all the $2$s from the array, and the array will become empty.</p>
