## Description

<div><p>You have a board represented as a grid with $2 \times n$ cells.</p><p>The first $k_1$ cells on the first row and first $k_2$ cells on the second row are colored in white. All other cells are colored in black.</p><p>You have $w$ white dominoes ($2 \times 1$ tiles, both cells are colored in white) and $b$ black dominoes ($2 \times 1$ tiles, both cells are colored in black).</p><p>You can place a white domino on the board if both board's cells are white and not occupied by any other domino. In the same way, you can place a black domino if both cells are black and not occupied by any other domino.</p><p>Can you place all $w + b$ dominoes on the board if you can place dominoes both horizontally and vertically?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 3000$)&nbsp;�� the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k_1$ and $k_2$ ($1 \le n \le 1000$; $0 \le k_1, k_2 \le n$).</p><p>The second line of each test case contains two integers $w$ and $b$ ($0 \le w, b \le n$).</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it's possible to place all $w + b$ dominoes on the board and <span class="tex-font-style-tt">NO</span>, otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 3000$)&nbsp;�� the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k_1$ and $k_2$ ($1 \le n \le 1000$; $0 \le k_1, k_2 \le n$).</p><p>The second line of each test case contains two integers $w$ and $b$ ($0 \le w, b \le n$).</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it's possible to place all $w + b$ dominoes on the board and <span class="tex-font-style-tt">NO</span>, otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p>

## Samples

```input1
5
1 0 1
1 0
1 1 1
0 0
3 0 0
1 3
4 3 1
2 2
5 4 3
3 1
```

```output1
NO
YES
NO
YES
YES
```




## Note

<p>In the first test case, $n = 1$, $k_1 = 0$ and $k_2 = 1$. It means that $2 \times 1$ board has black cell $(1, 1)$ and white cell $(2, 1)$. So, you can't place any white domino, since there is only one white cell.</p><p>In the second test case, the board of the same size $2 \times 1$, but both cell are white. Since $w = 0$ and $b = 0$, so you can place $0 + 0 = 0$ dominoes on the board.</p><p>In the third test case, board $2 \times 3$, but fully colored in black (since $k_1 = k_2 = 0$), so you can't place any white domino.</p><p>In the fourth test case, cells $(1, 1)$, $(1, 2)$, $(1, 3)$, and $(2, 1)$ are white and other cells are black. You can place $2$ white dominoes at positions $((1, 1), (2, 1))$ and $((1, 2), (1, 3))$ and $2$ black dominoes at positions $((1, 4), (2, 4))$ $((2, 2), (2, 3))$.</p>
