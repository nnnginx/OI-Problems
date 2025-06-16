## Description

<div><p>Sakurako has prepared a task for you:</p><p>She gives you an array of $n$ integers and allows you to choose $i$ and $j$ such that $i \neq j$ and $a_i \ge a_j$, and then assign $a_i = a_i - a_j$ or $a_i = a_i + a_j$. You can perform this operation any number of times for any $i$ and $j$, as long as they satisfy the conditions.</p><p>Sakurako asks you what is the maximum possible value of $mex_k$$^{\text{∗}}$ of the array after any number of operations.</p><div class="statement-footnote"><p>$^{\text{∗}}$$mex_k$ is the $k$-th non-negative integer that is absent in the array. For example, $mex_1(\{1,2,3 \})=0$, since $0$ is the first element that is not in the array, and $mex_2(\{0,2,4 \})=3$, since $3$ is the second element that is not in the array.</p></div></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1\le n\le 2\cdot 10^5,1\le k\le 10^9$) &nbsp;— the number of elements in the array and the value $k$ for $mex_k$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots,a_n$ ($1\le a_i\le 10^9$) &nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum $mex_k$ that can be achieved through the operations.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1\le n\le 2\cdot 10^5,1\le k\le 10^9$) &nbsp;— the number of elements in the array and the value $k$ for $mex_k$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots,a_n$ ($1\le a_i\le 10^9$) &nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum $mex_k$ that can be achieved through the operations.</p>





```input1|2,3,6,7,10,11
6
1 3
3
2 10
1 1
3 1
1 2 3
3 2
1 2 4
4 5
2 2 2 16
4 5
2 2 2 3
```




```output1
2
11
3
4
8
8
```


