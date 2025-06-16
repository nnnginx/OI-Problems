## Description

<div><p>The game field is a matrix of size $10^9 \times 10^9$, with a cell at the intersection of the $a$-th row and the $b$-th column denoted as ($a, b$).</p><p>There are $n$ monsters on the game field, with the $i$-th monster located in the cell ($x_i, y_i$), while the other cells are empty. No more than one monster can occupy a single cell.</p><p>You can move one monster to any cell on the field that is not occupied by another monster <span class="tex-font-style-bf">at most once</span> .</p><p>After that, you must select <span class="tex-font-style-bf">one</span> rectangle on the field; all monsters within the selected rectangle will be destroyed. You must pay $1$ coin for each cell in the selected rectangle.</p><p>Your task is to find the minimum number of coins required to destroy all the monsters.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of monsters on the field.</p><p>The following $n$ lines contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^9$)&nbsp;！ the coordinates of the cell with the $i$-th monster. All pairs ($x_i, y_i$) are distinct.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum cost to destroy all $n$ monsters.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of monsters on the field.</p><p>The following $n$ lines contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^9$)&nbsp;！ the coordinates of the cell with the $i$-th monster. All pairs ($x_i, y_i$) are distinct.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum cost to destroy all $n$ monsters.</p>





```input1|2,3,4,5,12,13,14,15,16,19,20,21,22,23,24,29,30,31,32,33
7
3
1 1
1 2
2 1
5
1 1
2 6
6 4
3 3
8 2
4
1 1
1 1000000000
1000000000 1
1000000000 1000000000
1
1 1
5
1 2
4 2
4 3
3 1
3 2
3
1 1
2 5
2 2
4
4 3
3 1
4 4
1 2
```




```output1
3
32
1000000000000000000
1
6
4
8
```



## Note

<p>Below are examples of optimal moves, with the cells of the rectangle to be selected highlighted in green.</p><center> <img class="tex-graphics" src="./37537/file/Hku7J3uv.png" style="zoom: 75.0%;max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Required move for the first example.</span> </center><center> <img class="tex-graphics" src="./37537/file/gOHMXIzR.png" style="zoom: 75.0%;max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Required move for the fifth example.</span> </center>
