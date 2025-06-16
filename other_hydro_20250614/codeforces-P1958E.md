## Description

<div><p>Suppose you have a permutation $p$ of $n$ integers ！ an array where each element is an integer from $1$ to $n$, and every integer from $1$ to $n$ appears exactly once.</p><p>In one operation, you remove <span class="tex-font-style-bf">every</span> element of this permutation which is less than at least one of its neighbors. For example, when you apply the operation to $[3, 1, 2, 5, 4]$, you get $[3, 5]$. If you apply an operation again, you get $[5]$.</p><p>It's easy to see that after applying a finite number of operations, you get an array consisting of a single integer $n$.</p><p>You are given two integers $n$ and $k$. Find a permutation of $n$ integers such that it becomes an array consisting of a single element $n$ after exactly $k$ operations (and not earlier).</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 2000$) ！ the number of test cases.</p><p>Each test case consists of one line containing two integers $n$ and $k$ ($2 \le n \le 100$; $1 \le k \le n - 1$).</p></div><div class="output-specification"><p>For each test case, print the answer as follows:</p><ul> <li> if a permutation of size $n$ which becomes an array consisting of a single element $n$ after exactly $k$ operations does not exist, print $-1$; </li><li> otherwise, print $n$ distinct integers from $1$ to $n$ ！ the requested permutation. If there are multiple such permutations, print any of them. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 2000$) ！ the number of test cases.</p><p>Each test case consists of one line containing two integers $n$ and $k$ ($2 \le n \le 100$; $1 \le k \le n - 1$).</p>

## Output

<p>For each test case, print the answer as follows:</p><ul> <li> if a permutation of size $n$ which becomes an array consisting of a single element $n$ after exactly $k$ operations does not exist, print $-1$; </li><li> otherwise, print $n$ distinct integers from $1$ to $n$ ！ the requested permutation. If there are multiple such permutations, print any of them. </li></ul>





```input1|2,4
4
5 2
5 4
2 1
3 2
```




```output1
3 1 2 5 4
-1
1 2
2 1 3
```


