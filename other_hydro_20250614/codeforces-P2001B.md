## Description

<div><p>There is an integer sequence $a$ of length $n$, where each element is initially $-1$.</p><p>Misuki has two typewriters where the first one writes letters from left to right, with a pointer initially pointing to $1$, and another writes letters from right to left with a pointer initially pointing to $n$.</p><p>Misuki would choose one of the typewriters and use it to perform the following operations until $a$ becomes a permutation of $[1, 2, \ldots, n]$</p><ul> <li> write number: write the minimum <span class="tex-font-style-bf">positive</span> integer that isn't present in the array $a$ to the element $a_i$, $i$ is the position where the pointer points at. Such operation can be performed only when $a_i = -1$. </li><li> carriage return: return the pointer to its initial position (i.e. $1$ for the first typewriter, $n$ for the second) </li><li> move pointer: move the pointer to the next position, let $i$ be the position the pointer points at before this operation, if Misuki is using the first typewriter, $i := i + 1$ would happen, and $i := i - 1$ otherwise. Such operation can be performed only if after the operation, $1 \le i \le n$ holds. </li></ul><p>Your task is to construct any permutation $p$ of length $n$, such that the minimum number of carriage return operations needed to make $a = p$ is the same no matter which typewriter Misuki is using.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 500$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the length of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a line of $n$ integers, representing the permutation $p$ of length $n$ such that the minimum number of carriage return operations needed to make $a = p$ is the same no matter which typewriter Misuki is using, or $-1$ if it is impossible to do so.</p><p>If there are multiple valid permutations, you can output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 500$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the length of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a line of $n$ integers, representing the permutation $p$ of length $n$ such that the minimum number of carriage return operations needed to make $a = p$ is the same no matter which typewriter Misuki is using, or $-1$ if it is impossible to do so.</p><p>If there are multiple valid permutations, you can output any of them.</p>





```input1
3
1
2
3
```




```output1
1
-1
3 1 2
```



## Note

<p>In the first testcase, it's possible to make $a = p = [1]$ using $0$ carriage return operations.</p><p>In the second testcase, it is possible to make $a = p = [1, 2]$ with the minimal number of carriage returns as follows:</p><p>If Misuki is using the first typewriter:</p><ul> <li> Write number: write $1$ to $a_1$, $a$ becomes $[1, -1]$ </li><li> Move pointer: move the pointer to the next position. (i.e. $2$) </li><li> Write number: write $2$ to $a_2$, $a$ becomes $[1, 2]$ </li></ul><p>If Misuki is using the second typewriter:</p><ul> <li> Move pointer: move the pointer to the next position. (i.e. $1$) </li><li> Write number: write $1$ to $a_1$, $a$ becomes $[1, -1]$ </li><li> Carriage return: return the pointer to $2$. </li><li> Write number: write $2$ to $a_2$, $a$ becomes $[1, 2]$ </li></ul><p>It can be proven that the minimum number of carriage returns needed to transform $a$ into $p$ when using the first typewriter is $0$ and it is $1$ when using the second one, so this permutation is not valid.</p><p>Similarly, $p = [2, 1]$ is also not valid, so there is no solution for $n = 2$.</p><p>In the third testcase, it is possibile to make $a = p = [3, 1, 2]$ with $1$ carriage return with both the first and the second typewriter. It can be proven that, for both typewriters, it is impossible to write $p$ with $0$ carriage returns.</p><p>With the first typewriter it is possible to: </p><ul> <li> Move pointer: move the pointer to the next position. (i.e. $2$) </li><li> Write number: write $1$ to $a_2$, $a$ becomes $[-1, 1, -1]$ </li><li> Move pointer: move the pointer to the next position. (i.e. $3$) </li><li> Write number: write $2$ to $a_3$, $a$ becomes $[-1, 1, 2]$ </li><li> Carriage return: return the pointer to $1$. </li><li> Write number: write $3$ to $a_1$, $a$ becomes $[3,1,2]$ </li></ul><p>With the second typewriter it is possible to: </p><ul> <li> Move pointer: move the pointer to the next position. (i.e. $2$) </li><li> Write number: write $1$ to $a_2$, $a$ becomes $[-1, 1, -1]$ </li><li> Carriage return: return the pointer to $3$. </li><li> Write number: write $2$ to $a_3$, $a$ becomes $[-1, 1, 2]$ </li><li> Move pointer: move the pointer to the next position. (i.e. $2$) </li><li> Move pointer: move the pointer to the next position. (i.e. $1$) </li><li> Write number: write $3$ to $a_1$, $a$ becomes $[3, 1, 2]$ </li></ul>
