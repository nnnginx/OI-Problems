## Description

<div><p>Baby Ehab is known for his love for a certain operation. He has an array $a$ of length $n$, and he decided to keep doing the following operation on it: </p><ul> <li> he picks $2$ adjacent elements; he then removes them and places a single integer in their place: their <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a>. Note that the length of the array decreases by one. </li></ul><p>Now he asks you if he can make all elements of the array equal. Since babies like to make your life harder, he requires that you leave at least $2$ elements remaining.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 15$)&nbsp;！ the number of test cases you need to solve.</p><p>The first line of each test case contains an integers $n$ ($2 \le n \le 2000$)&nbsp;！ the number of elements in the array $a$.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($0 \le a_i &lt; 2^{30}$)&nbsp;！ the elements of the array $a$.</p></div><div class="output-specification"><p>If Baby Ehab can make all elements equal while leaving at least $2$ elements standing, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 15$)&nbsp;！ the number of test cases you need to solve.</p><p>The first line of each test case contains an integers $n$ ($2 \le n \le 2000$)&nbsp;！ the number of elements in the array $a$.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\ldots$, $a_{n}$ ($0 \le a_i &lt; 2^{30}$)&nbsp;！ the elements of the array $a$.</p>

## Output

<p>If Baby Ehab can make all elements equal while leaving at least $2$ elements standing, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>

## Samples

```input1
2
3
0 2 2
4
2 3 1 10
```

```output1
YES
NO
```




## Note

<p>In the first sample, he can remove the first $2$ elements, $0$ and $2$, and replace them by $0 \oplus 2=2$. The array will be $[2,2]$, so all the elements are equal.</p><p>In the second sample, there's no way to make all the elements equal.</p>
