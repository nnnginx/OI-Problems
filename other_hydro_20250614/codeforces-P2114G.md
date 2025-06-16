## Description

<div><p>Yesterday, Dima found an empty array and decided to add some integers to it. He can perform the following operation an unlimited number of times:</p><ul> <li> add any integer to the left or right end of the array. </li><li> then, as long as there is a pair of identical adjacent elements in the array, they will be replaced by their sum. </li></ul><p>It can be shown that there can be at most one such pair in the array at the same time.</p><p>For example, if the array is $[3, 6, 4]$ and we add the number $3$ to the left, the array will first become $[3, 3, 6, 4]$, then the first two elements will be replaced by $6$, and the array will become $[6, 6, 4]$, and then ！ $[12, 4]$.</p><p>After performing the operation <span class="tex-font-style-bf">exactly</span> $k$ times, he thinks he has obtained an array $a$ of length $n$, but he does not remember which operations he applied. Determine if there exists a sequence of $k$ operations that could result in the given array $a$ from an empty array, or determine that it is impossible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case description contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $n \le k \le 10^6$) ！ the length of the resulting array and the number of operations.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 10^9, a_{i - 1} \ne a_i$) ！ the elements of the resulting array.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no suitable sequence of operations of length $k$, output "<span class="tex-font-style-tt">NO</span>". Otherwise, output "<span class="tex-font-style-tt">YES</span>".</p><p>You may output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case description contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $n \le k \le 10^6$) ！ the length of the resulting array and the number of operations.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 10^9, a_{i - 1} \ne a_i$) ！ the elements of the resulting array.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if there is no suitable sequence of operations of length $k$, output "<span class="tex-font-style-tt">NO</span>". Otherwise, output "<span class="tex-font-style-tt">YES</span>".</p><p>You may output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11,14,15
8
3 3
2 1 4
3 7
2 1 4
2 15
2 16
3 10
256 32 1
3 289
768 96 1
3 290
768 96 1
5 7
5 1 6 3 10
4 6
6 8 5 10
```




```output1
YES
NO
YES
YES
YES
NO
YES
YES
```


