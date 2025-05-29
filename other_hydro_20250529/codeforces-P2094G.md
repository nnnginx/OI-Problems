## Description

<div><p><span class="tex-font-style-it">Chimpanzini Bananini stands on the brink of a momentous battle！one destined to bring finality.</span></p><p>For an arbitrary array $b$ of length $m$, let's denote the <span class="tex-font-style-it">rizziness</span> of the array to be $\sum_{i=1}^mb_i\cdot i=b_1\cdot 1+b_2\cdot 2+b_3\cdot 3+\ldots + b_m\cdot m$.</p><p>Chimpanzini Bananini gifts you an empty array. There are three types of operations you can perform on it. </p><ol> <li> Perform a cyclic shift on the array. That is, the array $[a_1, a_2, \ldots, a_n]$ becomes $[a_n, a_1, a_2, \ldots, a_{n-1}].$ </li><li> Reverse the entire array. That is, the array $[a_1, a_2, \ldots, a_n]$ becomes $[a_n, a_{n-1}, \ldots, a_1].$ </li><li> Append an element to the end of the array. The array $[a_1, a_2, \ldots, a_n]$ becomes $[a_1, a_2, \ldots, a_n, k]$ after appending $k$ to the end of the array. </li></ol><p>After each operation, you are interested in calculating the <span class="tex-font-style-it">rizziness</span> of your array. </p><p>Note that all operations are <span class="tex-font-style-bf">persistent</span>. This means that each operation modifies the array, and subsequent operations should be applied to the current state of the array after the previous operations.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of the input contains an integer $q$ ($1 \leq q \leq 2\cdot 10^5$)&nbsp;！ the number of operations you perform on your array.</p><p>The following $q$ lines first contain a single integer $s$ ($1 \leq s \leq 3$)&nbsp;！ the operation type. </p><ul> <li> If $s=1$, then the cyclic shift operation should be performed. </li><li> If $s=2$, then the reversal operation should be performed. </li><li> If $s=3$, then the line will contain an additional integer $k$ ($1 \leq k \leq 10^6$), denoting the element appended to the back of the array. </li></ul><p>It is guaranteed that the sum of $q$ will not exceed $2\cdot 10^5$ over all test cases. Additionally, it is guaranteed that the first operation on each test case will be one with $s=3$.</p></div><div class="output-specification"><p>For each test case, output $q$ lines, outputting the <span class="tex-font-style-it">rizziness</span> of your array after each operation.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of the input contains an integer $q$ ($1 \leq q \leq 2\cdot 10^5$)&nbsp;！ the number of operations you perform on your array.</p><p>The following $q$ lines first contain a single integer $s$ ($1 \leq s \leq 3$)&nbsp;！ the operation type. </p><ul> <li> If $s=1$, then the cyclic shift operation should be performed. </li><li> If $s=2$, then the reversal operation should be performed. </li><li> If $s=3$, then the line will contain an additional integer $k$ ($1 \leq k \leq 10^6$), denoting the element appended to the back of the array. </li></ul><p>It is guaranteed that the sum of $q$ will not exceed $2\cdot 10^5$ over all test cases. Additionally, it is guaranteed that the first operation on each test case will be one with $s=3$.</p>

## Output

<p>For each test case, output $q$ lines, outputting the <span class="tex-font-style-it">rizziness</span> of your array after each operation.</p>





```input1|2,3,4,5,6,7,8,9,10,11,12,13,14,15
1
13
3 1
3 2
3 3
1
3 4
2
3 5
1
3 6
2
3 7
2
1
```




```output1
1
5
14
11
27
23
48
38
74
73
122
102
88
```



## Note

<p>The first six states of the array: </p><ul> <li> $[1]$ </li><li> $[1, 2]$ </li><li> $[1, 2, 3]$ </li><li> $[3, 1, 2]$ </li><li> $[3, 1, 2, 4]$ </li><li> $[4, 2, 1, 3]$ </li></ul>
