## Description

<div><p>Sakurako will soon take a test. The test can be described as an array of integers $n$ and a task on it:</p><p>Given an integer $x$, Sakurako can perform the following operation any number of times:</p><ul> <li> Choose an integer $i$ ($1\le i\le n$) such that $a_i\ge x$; </li><li> Change the value of $a_i$ to $a_i-x$. </li></ul><p>Using this operation any number of times, she must find the minimum possible median$^{\text{∗}}$ of the array $a$.</p><p>Sakurako knows the array but does not know the integer $x$. Someone let it slip that one of the $q$ values of $x$ will be in the next test, so Sakurako is asking you what the answer is for each such $x$.</p><div class="statement-footnote"><p>$^{\text{∗}}$The median of an array of length $n$ is the element that stands in the middle of the sorted array (at the $\frac{n+2}{2}$-th position for even $n$, and at the $\frac{n+1}{2}$-th for odd)</p></div></div><div class="input-specification"><p>The first line contains one integer $t$ ($1\le t\le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1\le n,q\le 10^5$) &nbsp;— the number of elements in the array and the number of queries.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1\le a_i\le n$) &nbsp;— the elements of the array.</p><p>The following $q$ lines each contain one integer $x$ ($1\le x\le n$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^5$. The same guarantee applies to the sum of $q$ across all test cases.</p></div><div class="output-specification"><p>For each test case, output $q$ integers &nbsp;— the answer for each query.</p></div>

## Input

<p>The first line contains one integer $t$ ($1\le t\le 10^4$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1\le n,q\le 10^5$) &nbsp;— the number of elements in the array and the number of queries.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1\le a_i\le n$) &nbsp;— the elements of the array.</p><p>The following $q$ lines each contain one integer $x$ ($1\le x\le n$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^5$. The same guarantee applies to the sum of $q$ across all test cases.</p>

## Output

<p>For each test case, output $q$ integers &nbsp;— the answer for each query.</p>





```input1|2,3,4,5,6,7,8
2
5 5
1 2 3 4 5
1
2
3
4
5
6 3
1 2 6 4 1 3
2
1
5
```




```output1
0 1 1 1 2 
1 0 2
```


