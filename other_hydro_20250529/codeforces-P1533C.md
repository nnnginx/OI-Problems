## Description

<div><p>Anya came to her friend's birthday party. There are $n$ delicious sweets on a circle table (for convenience, we will number them from $1$ to $n$ in clockwise direction). For each of the sweets, it is known whether Anya likes it or not. Anya decided that she should eat all the sweets that are on the table, and she likes them.</p><p>However, eating all the sweets in some random order is too boring. Therefore, Anya came up with a game that will make the process of eating sweets more interesting.</p><p>The game is played according to the following rules:</p><ul> <li> if there are no sweets that Anya likes left on the table, then the game ends; </li><li> at the very beginning of the game, if there is at least one sweet on the table that Anya wants to eat, she eats the sweet number $1$; </li><li> after Anya has eaten some sweet, she counts $k$ sweets clockwise, starting from the next sweet in the circle, and eats the $k$-th sweet in the count (if there are less than $k$ sweets in the circle, some sweets can participate in the count more than once, and the last sweet in the count is picked). Obviously, the sweets that have already been eaten do not participate in the count. </li></ul><p>For example, let $6$ sweets be arranged in a circle, Anya likes sweets $4$, $5$ and $6$, $k = 4$. Then the game goes as follows:</p><ol> <li> initially there are sweets $[1, 2, 3, 4, 5, 6]$ on the table, Anya chooses the sweet number $1$. </li><li> Anya eats the sweet number $1$, after that, there are sweets $[2, 3, 4, 5, 6]$ on the table. Anya counts $4$ sweets, starting with the $2$-nd sweet, and stops at the $5$-th sweet. </li><li> Anya eats the $5$-th sweet, after that, there are sweets $[2, 3, 4, 6]$ on the table. Anya counts $4$ sweets, starting with the $6$-th sweet, and stops at the $4$-th sweet. </li><li> Anya eats the sweet number $4$, after that, there are sweets $[2, 3, 6]$ on the table. Anya counts $4$ sweets, starting with the $6$-th sweet, and stops at the $6$-th sweet. </li><li> Anya eats the sweet number $6$, after that, there are sweets $[2, 3]$ on the table. There are no sweets that Anya likes on the table, so the game ends. </li></ol><p>Your task is to calculate the number of sweets that Anya will eat.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$)&nbsp;！ the number of sweets and the parameter $k$.</p><p>The next line contains the string $s$, where $s_i = 1$ if Anya likes $i$-th sweet, and $s_i = 0$ otherwise.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;！ the number of sweets that Anya will eat.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$)&nbsp;！ the number of sweets and the parameter $k$.</p><p>The next line contains the string $s$, where $s_i = 1$ if Anya likes $i$-th sweet, and $s_i = 0$ otherwise.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, print one integer&nbsp;！ the number of sweets that Anya will eat.</p>

## Samples

```input1
4
6 4
000111
7 3
0000100
3 2
000
5 1
10011
```

```output1
4
4
0
5
```




## Note

<p>The first test case of the example is described in the statement.</p>
