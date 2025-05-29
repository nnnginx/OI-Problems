## Description

<div><p>For an array of integers $a_1, a_2, \dots, a_n$, we define its <span class="tex-font-style-bf">equality characteristic</span> as the array $b_2, b_3, \dots, b_{n-1}$, where $b_i = 1$ if the $i$-th element of the array $a$ is equal to both of its neighbors, and $b_i = 0$ if the $i$-th element of the array $a$ is not equal to at least one of its neighbors.</p><p>For example, for the array $[1, 2, 2, 2, 3, 3, 4, 4, 4, 4]$, the equality characteristic will be $[0, 1, 0, 0, 0, 0, 1, 1]$.</p><p>You are given the array $b_2, b_3, \dots, b_{n-1}$. Your task is to determine whether there exists such an array $a$ for which the given array is the equality characteristic.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) ¡ª the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($3 \le n \le 100$); </li><li> the second line contains $n-2$ integers $b_2, b_3, \dots, b_{n-1}$ ($0 \le b_i \le 1$). </li></ul></div><div class="output-specification"><p>For each test case, output <span class="tex-font-style-tt">YES</span> if the array $a$ exists, or <span class="tex-font-style-tt">NO</span> if such an array does not exist. Each letter can be printed in any case.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) ¡ª the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($3 \le n \le 100$); </li><li> the second line contains $n-2$ integers $b_2, b_3, \dots, b_{n-1}$ ($0 \le b_i \le 1$). </li></ul>

## Output

<p>For each test case, output <span class="tex-font-style-tt">YES</span> if the array $a$ exists, or <span class="tex-font-style-tt">NO</span> if such an array does not exist. Each letter can be printed in any case.</p>





```input1|2,3,6,7
3
10
0 1 0 0 0 0 1 1
3
1
10
0 1 0 1 1 0 0 1
```




```output1
YES
YES
NO
```



## Note

<p>In the first example, the array $a = [1, 2, 2, 2, 3, 3, 4, 4, 4, 4]$ is suitable.</p><p>In the second example, the array $a = [7, 7, 7]$ is suitable.</p>
