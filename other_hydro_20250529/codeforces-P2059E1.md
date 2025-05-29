## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is that in this version you only need to find the minimum number of operations. You can hack only if you solved all versions of this problem.</span></p><p>You are given $n$ arrays, each of which has a length of $m$. Let the $j$-th element of the $i$-th array be denoted as $a_{i, j}$. It is guaranteed that all $a_{i, j}$ are <span class="tex-font-style-bf">pairwise distinct</span>. In one operation, you can do the following:</p><ul> <li> Choose some integer $i$ ($1 \le i \le n$) and an integer $x$ ($1 \le x \le 2 \cdot n \cdot m$). </li><li> For all integers $k$ from $i$ to $n$ in increasing order, do the following: <ol> <li> Add the element $x$ to the beginning of the $k$-th array.<p> </p></li><li> Assign $x$ the value of the last element in the $k$-th array.<p> </p></li><li> Remove the last element from the $k$-th array. </li></ol></li></ul><p>In other words, you can insert an element at the beginning of any array, after which all elements in this and all following arrays are shifted by one to the right. The last element of the last array is removed.</p><p>You are also given a description of the arrays that need to be obtained after all operations. That is, after performing the operations, the $j$-th element of the $i$-th array should be equal to $b_{i, j}$. It is guaranteed that all $b_{i, j}$ are <span class="tex-font-style-bf">pairwise distinct</span>.</p><p>Determine the minimum number of operations that need to be performed to obtain the desired arrays.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 3 \cdot 10^5$)&nbsp;！ the number of arrays and the number of elements in each array.</p><p>The $i$-th of the following $n$ lines contains $m$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, m}$ ($1 \le a_{i, j} \le 2 \cdot n \cdot m$)&nbsp;！ the elements of the $i$-th original array. It is guaranteed that all $a_{i, j}$ are pairwise distinct.</p><p>The $i$-th of the following $n$ lines contains $m$ integers $b_{i, 1}, b_{i, 2}, \ldots, b_{i, m}$ ($1 \le b_{i, j} \le 2 \cdot n \cdot m$)&nbsp;！ the elements of the $i$-th final array. It is guaranteed that all $b_{i, j}$ are pairwise distinct.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of operations that need to be performed.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 3 \cdot 10^5$)&nbsp;！ the number of arrays and the number of elements in each array.</p><p>The $i$-th of the following $n$ lines contains $m$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, m}$ ($1 \le a_{i, j} \le 2 \cdot n \cdot m$)&nbsp;！ the elements of the $i$-th original array. It is guaranteed that all $a_{i, j}$ are pairwise distinct.</p><p>The $i$-th of the following $n$ lines contains $m$ integers $b_{i, 1}, b_{i, 2}, \ldots, b_{i, m}$ ($1 \le b_{i, j} \le 2 \cdot n \cdot m$)&nbsp;！ the elements of the $i$-th final array. It is guaranteed that all $b_{i, j}$ are pairwise distinct.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of operations that need to be performed.</p>





```input1|2,3,4,5,6,10,11,12,13,14,15,16
4
2 2
2 6
3 4
1 2
7 8
1 5
5 4 1 2 3
5 4 3 2 1
3 3
1 2 3
4 5 6
7 8 9
11 1 2
12 3 4
13 5 6
4 4
1 2 3 4
5 6 7 8
9 10 11 12
13 14 15 16
17 1 2 3
4 18 5 6
7 19 8 20
9 21 22 10
```




```output1
3
5
3
6
```



## Note

<p>In the first test case, the following sequence of $3$ operations is suitable:</p><ul> <li> Apply the operation to the first array with $x = 1$. Then the element $1$ will be added to the beginning of the first array, and the value of $x$ will become $6$. The last element will be removed, and the first array will look like $[1, 2]$. Next, the element $x$ is added to the beginning of the second array, and the value of $x$ becomes $4$. The last element of the second array is removed, and both arrays look like $[1, 2]$ and $[6, 3]$ respectively after the first operation.</li><li> Apply the operation to the second array with $x = 8$. Then the first array remains unchanged, and both arrays will look like $[1, 2]$ and $[8, 6]$ respectively.</li><li> Apply the operation to the second array with $x = 7$, then both arrays will have the required appearance $[1, 2]$ and $[7, 8]$ respectively. </li></ul><p>In the second test case, the desired array can only be achieved in $5$ operations.</p><p>In the third test case, the following sequence of $3$ operations is suitable:</p><ul> <li> Apply the operation with $x = 11$ to the first array.</li><li> Apply the operation with $x = 12$ to the second array.</li><li> Apply the operation with $x = 13$ to the third array. </li></ul>
