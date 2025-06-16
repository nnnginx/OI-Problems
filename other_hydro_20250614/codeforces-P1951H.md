## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/3WWwuA6twKI"><span class="tex-font-style-it">Piotr Rubik - Psalm dla Ciebie</span></a></div><div class="epigraph-source">ඞ</div></div><p>There is an array $a$ of size $2^k$ for some positive integer $k$, which is initially a permutation of values from $1$ to $2^k$. Alice and Bob play the following game on the array $a$. First, a value $t$ between $1$ and $k$ is shown to both Alice and Bob. Then, for exactly $t$ turns, the following happens: </p><ul> <li> Alice either does nothing, or chooses two distinct elements of the array $a$ and swaps them. </li><li> Bob chooses either the left half or the right half of the array $a$ and erases it. </li></ul><p>The score of the game is defined as the maximum value in $a$ after all $t$ turns have been played. Alice wants to maximize this score, while Bob wants to minimize it.</p><p>You need to output $k$ numbers: the score of the game if both Alice and Bob play optimally for $t$ from $1$ to $k$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $k$ ($1 \le k \le 20$)&nbsp;— the parameter of the size of $a$.</p><p>The second line of each test case contains $2^k$ integers $a_1, a_2, \ldots, a_{2^k}$ ($1 \le a_i \le 2^k$, $a_i$'s are pairwise distinct)&nbsp;— the given array $a$.</p><p>It is guaranteed that the sum of $2^k$ over all test cases does not exceed $2^{20}$.</p></div><div class="output-specification"><p>For each test case, print $k$ numbers, where the $i$-th number is the score of the game if both Alice and Bob play optimally for $t = i$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $k$ ($1 \le k \le 20$)&nbsp;— the parameter of the size of $a$.</p><p>The second line of each test case contains $2^k$ integers $a_1, a_2, \ldots, a_{2^k}$ ($1 \le a_i \le 2^k$, $a_i$'s are pairwise distinct)&nbsp;— the given array $a$.</p><p>It is guaranteed that the sum of $2^k$ over all test cases does not exceed $2^{20}$.</p>

## Output

<p>For each test case, print $k$ numbers, where the $i$-th number is the score of the game if both Alice and Bob play optimally for $t = i$.</p>





```input1|2,3,6,7,10,11
5
1
1 2
2
4 3 2 1
3
5 1 6 4 7 2 8 3
4
10 15 6 12 1 3 4 9 13 5 7 16 14 11 2 8
5
32 2 5 23 19 17 31 7 29 3 4 16 13 9 30 24 14 1 8 20 6 15 26 18 10 27 22 12 25 21 28 11
```




```output1
1
3 1
7 5 1
15 13 9 1
31 28 25 17 1
```



## Note

<p>In the third test case, for $t = 2$, the game could have proceeded as follows: </p><ul> <li> Initially, $a = [5, 1, 6, 4, 7, 2, 8, 3]$. </li><li> Alice swaps $a_6$ and $a_8$, $a$ becomes $[5, 1, 6, 4, 7, 3, 8, 2]$. </li><li> Bob erases the right half of the array, $a$ becomes $[5, 1, 6, 4]$. </li><li> Alice does nothing, $a$ remains as $[5, 1, 6, 4]$. </li><li> Bob erases the right half of the array, $a$ becomes $[5, 1]$. </li><li> The game ends with a score of $5$. </li></ul>
