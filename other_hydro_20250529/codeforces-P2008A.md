## Description

<div><p>Today, Sakurako has a math exam. The teacher gave the array, consisting of $a$ ones and $b$ twos.</p><p>In an array, Sakurako <span class="tex-font-style-bf">must</span> place either a '<span class="tex-font-style-tt">+</span>' or a '<span class="tex-font-style-tt">-</span>' in front of each element so that the sum of all elements in the array equals $0$.</p><p>Sakurako is not sure if it is possible to solve this problem, so determine whether there is a way to assign signs such that the sum of all elements in the array equals $0$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 100$) &nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $a$ and $b$ ($0\le a,b&lt;10$) &nbsp;！ the number of '1's and the number of '2's in the array.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if you can make the sum of the entire array equal to $0$, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 100$) &nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $a$ and $b$ ($0\le a,b&lt;10$) &nbsp;！ the number of '1's and the number of '2's in the array.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if you can make the sum of the entire array equal to $0$, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,4,6
5
0 1
0 3
2 0
2 3
3 1
```




```output1
NO
NO
YES
YES
NO
```



## Note

<ol> <li> $a=0$, $b=1$: This means the array is $[2]$ ！ it is impossible to add the signs '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>' to get $0$ as a result;</li><li> $a=0$, $b=3$: This means the array is $[2, 2, 2]$ ！ it is impossible to add the signs '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>' to get $0$ as a result;</li><li> $a=2$, $b=0$: This means the array is $[1, 1]$ ！ it is possible to add the signs '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>' to get $0$ as a result ($+1-1=0$);</li><li> $a=2$, $b=3$: This means the array is $[1, 1, 2, 2, 2]$ ！ it is possible to add the signs '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>' to get $0$ as a result ($+1+1-2-2+2=0$);</li></ol>
