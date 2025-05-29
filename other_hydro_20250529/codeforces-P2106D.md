## Description

<div><p>Flower boy has a garden of $n$ flowers that can be represented as an integer sequence $a_1, a_2, \dots, a_n$, where $a_i$ is the beauty of the $i$-th flower from the left.</p><p>Igor wants to collect exactly $m$ flowers. To do so, he will walk the garden <span class="tex-font-style-bf">from left to right</span> and choose whether to collect the flower at his current position. The $i$-th flower among ones he collects must have a beauty of <span class="tex-font-style-bf">at least</span> $b_i$.</p><p>Igor noticed that it might be impossible to collect $m$ flowers that satisfy his beauty requirements, so <span class="tex-font-style-bf">before</span> he starts collecting flowers, he can pick any integer $k$ and use his magic wand to grow a new flower with beauty $k$ and place it <span class="tex-font-style-bf">anywhere</span> in the garden (between two flowers, before the first flower, or after the last flower). Because his magic abilities are limited, he may do this <span class="tex-font-style-bf">at most once</span>.</p><p>Output the <span class="tex-font-style-bf">minimum</span> integer $k$ Igor must pick when he performs the aforementioned operation to ensure that he can collect $m$ flowers. If he can collect $m$ flowers without using the operation, output $0$. If it is impossible to collect $m$ flowers despite using the operation, output $-1$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \le t \le 10^4)$&nbsp;！ the number of test cases.</p><p>The first line of each test case contains exactly two integers $n$ and $m$ $(1 \le m \le n \le 2 \cdot 10^5)$&nbsp;！ the number of flowers in the garden and the number of flowers Igor wants to collect, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, ..., a_n$ $(1 \le a_i \le 10^9)$&nbsp;！ where $a_i$ is the beauty of the $i$-th flower from the left in the garden.</p><p>The third line of each test case contains $m$ integers $b_1, b_2, ..., b_m$ $(1 \le b_i \le 10^9)$&nbsp;！ where $b_i$ is the minimum beauty the $i$-th flower must have that Igor will collect.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, on a separate line, output the minimum integer $k$ Igor must pick when he performs the aforementioned operation to ensure that he can collect $m$ flowers. If he can collect $m$ flowers without using the operation, output $0$. If it is impossible to collect $m$ flowers despite using the operation, output $-1$.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \le t \le 10^4)$&nbsp;！ the number of test cases.</p><p>The first line of each test case contains exactly two integers $n$ and $m$ $(1 \le m \le n \le 2 \cdot 10^5)$&nbsp;！ the number of flowers in the garden and the number of flowers Igor wants to collect, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, ..., a_n$ $(1 \le a_i \le 10^9)$&nbsp;！ where $a_i$ is the beauty of the $i$-th flower from the left in the garden.</p><p>The third line of each test case contains $m$ integers $b_1, b_2, ..., b_m$ $(1 \le b_i \le 10^9)$&nbsp;！ where $b_i$ is the minimum beauty the $i$-th flower must have that Igor will collect.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, on a separate line, output the minimum integer $k$ Igor must pick when he performs the aforementioned operation to ensure that he can collect $m$ flowers. If he can collect $m$ flowers without using the operation, output $0$. If it is impossible to collect $m$ flowers despite using the operation, output $-1$.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
7
9 5
3 5 2 3 3 5 8 1 2
4 6 2 4 6
6 3
1 2 6 8 2 1
5 4 3
5 3
4 3 5 4 3
7 4 5
6 3
8 4 2 1 2 5
6 1 4
5 5
1 2 3 4 5
5 4 3 2 1
6 3
1 2 3 4 5 6
9 8 7
5 5
7 7 6 7 7
7 7 7 7 7
```




```output1
6
3
7
0
-1
-1
7
```



## Note

<p>In the first test case, suppose Igor grows a flower of beauty $6$ and places it between the third and the fourth flowers. Then, the garden will look like the following: $[3, 5, 2, 6, 3, 3, 5, 8, 1, 2]$. Then, he can select the second, fourth, sixth, seventh, and eighth flowers with beauties $[5, 6, 3, 5, 8]$. </p><p>In the third test case, he can grow a flower of beauty $7$ and place it before the first flower. The garden will look like the following: $[7, 4, 3, 5, 4, 3]$. Now, he can choose the first, second, and fourth flowers.</p><p>In the fourth test case, Igor does not need to use the operation, so the answer is $0$.</p><p>In the sixth test case, no matter how Igor performs the operation, he cannot collect $3$ flowers such that the $i$-th flower he collects has a beauty of at least $b_i$, therefore the answer is $-1$.</p>
