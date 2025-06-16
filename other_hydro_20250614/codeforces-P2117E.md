## Description

<div><p>You are given two integer arrays $a$ and $b$, each of length $n$.</p><p>You may perform the following operation any number of times: </p><ul> <li> Choose an index $i$ $(1 \le i \le n - 1)$, and set $a_i := b_{i + 1}$, <span class="tex-font-style-bf">or</span> set $b_i := a_{i + 1}$. </li></ul><p><span class="tex-font-style-bf">Before</span> performing any operations, you are allowed to choose an index $i$ $(1 \le i \le n)$ and remove both $a_i$ and $b_i$ from the arrays. This removal can be done <span class="tex-font-style-bf">at most once</span>.</p><p>Let the number of matches between two arrays $c$ and $d$ of length $m$ be the number of positions $j$ $(1 \le j \le m)$ such that $c_j = d_j$.</p><p>Your task is to compute the maximum number of matches you can achieve.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ $(1 \le t \le 10^4)$ ！ the number of test cases. The description of each test case follows.</p><p>The first line contains an integer $n$ $(2 \le n \le 2 \cdot 10^5)$ ！ the length of $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le n)$ ！ the elements of $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ $(1 \le b_i \le n)$ ！ the elements of $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer ！ the answer for the test case.</p></div>

## Input

<p>The first line of the input contains an integer $t$ $(1 \le t \le 10^4)$ ！ the number of test cases. The description of each test case follows.</p><p>The first line contains an integer $n$ $(2 \le n \le 2 \cdot 10^5)$ ！ the length of $a$ and $b$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le n)$ ！ the elements of $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ $(1 \le b_i \le n)$ ！ the elements of $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer ！ the answer for the test case.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22,26,27,28
10
4
1 3 1 4
4 3 2 2
6
2 1 5 3 6 4
3 2 4 5 1 6
2
1 2
2 1
6
2 5 1 3 6 4
3 5 2 3 4 6
4
1 3 2 2
2 1 3 4
8
3 1 4 6 2 2 5 7
4 2 3 7 1 1 6 5
10
5 1 2 7 3 9 4 10 6 8
6 2 3 6 4 10 5 1 7 9
5
3 2 4 1 5
2 4 5 1 3
7
2 2 6 4 1 3 5
3 1 6 5 1 4 2
5
4 1 3 2 5
3 2 1 5 4
```




```output1
3
3
0
4
3
5
6
4
5
2
```



## Note

<p>In the first test case, we can do the following: </p><ul> <li> We will choose not to remove any index. </li><li> Choose index $3$, and set $a_3 := b_4$. The arrays become: $a = [1, 3, 2, 4]$, $b = [4, 3, 2, 2]$. </li><li> Choose index $1$, and set $a_1 := b_2$. The arrays become: $a = [3, 3, 2, 4]$, $b = [4, 3, 2, 2]$. </li><li> Choose index $1$, and set $b_1 := a_2$. The arrays become: $a = [3, 3, 2, 4]$, $b = [3, 3, 2, 2]$. Notice that you can perform $a_i := b_{i + 1}$ and $b_i := a_{i + 1}$ on the same index $i$. </li></ul><p>The number of matches is $3$. It can be shown that this is the maximum answer we can achieve.</p><p>In the second test case, we can do the following to achieve a maximum of $3$: </p><ul> <li> Let's choose to remove index $5$. The arrays become: $a = [2, 1, 5, 3, 4]$, $b = [3, 2, 4, 5, 6]$. </li><li> Choose index $4$, and set $b_4 := a_5$. The arrays become: $a = [2, 1, 5, 3, 4]$, $b = [3, 2, 4, 4, 6]$. </li><li> Choose index $3$, and set $a_3 := b_4$. The arrays become: $a = [2, 1, 4, 3, 4]$, $b = [3, 2, 4, 4, 6]$. </li><li> Choose index $2$, and set $a_2 := b_3$. The arrays become: $a = [2, 4, 4, 3, 4]$, $b = [3, 2, 4, 4, 6]$. </li><li> Choose index $1$, and set $b_1 := a_2$. The arrays become: $a = [2, 4, 4, 3, 4]$, $b = [4, 2, 4, 4, 6]$. </li><li> Choose index $2$, and set $b_2 := a_3$. The arrays become: $a = [2, 4, 4, 3, 4]$, $b = [4, 4, 4, 4, 6]$. </li><li> Choose index $1$, and set $a_1 := b_2$. The arrays become: $a = [4, 4, 4, 3, 4]$, $b = [4, 4, 4, 4, 6]$. </li></ul><p>In the third test case, it can be shown that we can not get any matches. Therefore, the answer is $0$.</p>
