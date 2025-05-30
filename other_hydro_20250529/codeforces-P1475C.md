## Description

<div><p>At the school where Vasya is studying, preparations are underway for the graduation ceremony. One of the planned performances is a ball, which will be attended by pairs of boys and girls.</p><p>Each class must present two couples to the ball. In Vasya's class, $a$ boys and $b$ girls wish to participate. But not all boys and not all girls are ready to dance in pairs.</p><p>Formally, you know $k$ possible one-boy-one-girl pairs. You need to choose two of these pairs so that no person is in more than one pair.</p><p>For example, if $a=3$, $b=4$, $k=4$ and the couples $(1, 2)$, $(1, 3)$, $(2, 2)$, $(3, 4)$ are ready to dance together (in each pair, the boy's number comes first, then the girl's number), then the following combinations of two pairs are possible (not all possible options are listed below): </p><ul> <li> $(1, 3)$ and $(2, 2)$; </li><li> $(3, 4)$ and $(1, 3)$; </li></ul><p>But the following combinations are not possible: </p><ul> <li> $(1, 3)$ and $(1, 2)$&nbsp;！ the first boy enters two pairs; </li><li> $(1, 2)$ and $(2, 2)$&nbsp;！ the second girl enters two pairs; </li></ul><p>Find the number of ways to select two pairs that match the condition above. Two ways are considered different if they consist of different pairs.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains three integers $a$, $b$ and $k$ ($1 \le a, b, k \le 2 \cdot 10^5$)&nbsp;！ the number of boys and girls in the class and the number of couples ready to dance together.</p><p>The second line of each test case contains $k$ integers $a_1, a_2, \ldots a_k$. ($1 \le a_i \le a$), where $a_i$ is the number of the boy in the pair with the number $i$.</p><p>The third line of each test case contains $k$ integers $b_1, b_2, \ldots b_k$. ($1 \le b_i \le b$), where $b_i$ is the number of the girl in the pair with the number $i$.</p><p>It is guaranteed that the sums of $a$, $b$, and $k$ over all test cases do not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that each pair is specified at most once in one test case.</p></div><div class="output-specification"><p>For each test case, on a separate line print one integer&nbsp;！ the number of ways to choose two pairs that match the condition above.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains three integers $a$, $b$ and $k$ ($1 \le a, b, k \le 2 \cdot 10^5$)&nbsp;！ the number of boys and girls in the class and the number of couples ready to dance together.</p><p>The second line of each test case contains $k$ integers $a_1, a_2, \ldots a_k$. ($1 \le a_i \le a$), where $a_i$ is the number of the boy in the pair with the number $i$.</p><p>The third line of each test case contains $k$ integers $b_1, b_2, \ldots b_k$. ($1 \le b_i \le b$), where $b_i$ is the number of the girl in the pair with the number $i$.</p><p>It is guaranteed that the sums of $a$, $b$, and $k$ over all test cases do not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that each pair is specified at most once in one test case.</p>

## Output

<p>For each test case, on a separate line print one integer&nbsp;！ the number of ways to choose two pairs that match the condition above.</p>

## Samples

```input1
3
3 4 4
1 1 2 3
2 3 2 4
1 1 1
1
1
2 2 4
1 1 2 2
1 2 1 2
```

```output1
4
0
2
```




## Note

<p>In the first test case, the following combinations of pairs fit: </p><ul> <li> $(1, 2)$ and $(3, 4)$; </li><li> $(1, 3)$ and $(2, 2)$; </li><li> $(1, 3)$ and $(3, 4)$; </li><li> $(2, 2)$ and $(3, 4)$. </li></ul><p>There is only one pair in the second test case.</p><p>In the third test case, the following combinations of pairs fit: </p><ul> <li> $(1, 1)$ and $(2, 2)$; </li><li> $(1, 2)$ and $(2, 1)$. </li></ul>
