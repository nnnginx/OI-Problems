## Description

<div><p>You have $n$ chips, and you are going to place all of them in one of $x$ points, numbered from $1$ to $x$. There can be multiple chips in each point.</p><p>After placing the chips, you can perform the following four operations (in any order, any number of times):</p><ul> <li> choose a chip in point $i \ge 3$, remove it and place two chips: one in $i-1$, one in $i-2$; </li><li> choose two chips in adjacent points $i$ and $i+1$, remove them and place a new chip in $i+2$; </li><li> choose a chip in point $1$ and move it to $2$; </li><li> choose a chip in point $2$ and move it to $1$. </li></ul><p>Note that the coordinates of the chips you place during the operations cannot be less than $1$, but can be greater than $x$.</p><p>Denote the <span class="tex-font-style-it">cost</span> of chip placement as the <span class="tex-font-style-bf">minimum</span> number of chips which can be present on the line after you perform these operations, starting from the placement you've chosen.</p><p>For example, the <span class="tex-font-style-it">cost</span> of placing two chips in points $3$ and one chip in point $5$ is $2$, because you can reduce the number of chips to $2$ as follows:</p><ul> <li> choose a chip in point $3$, remove it, place a chip in $1$ and another chip in $2$; </li><li> choose the chips in points $2$ and $3$, remove them and place a chip in $4$; </li><li> choose the chips in points $4$ and $5$, remove them and place a chip in $6$. </li></ul><p>You are given three integers $n$, $x$ and $m$. Calculate the number of placements of exactly $n$ chips in points from $1$ to $x$ having cost equal to $m$, and print it modulo $998244353$. Two placements are considered different if the number of chips in some point differs between these placements.</p></div><div class="input-specification"><p>The only line contains three integers $n$, $x$ and $m$ ($1 \le m \le n \le 1000$; $2 \le x \le 10$).</p></div><div class="output-specification"><p>Print one integer ¡ª the number of placements with cost equal to $m$, taken modulo $998244353$.</p></div>

## Input

<p>The only line contains three integers $n$, $x$ and $m$ ($1 \le m \le n \le 1000$; $2 \le x \le 10$).</p>

## Output

<p>Print one integer ¡ª the number of placements with cost equal to $m$, taken modulo $998244353$.</p>





```input1|
2 3 1
```




```input2|
42 10 5
```




```input3|
1000 10 8
```




```output1
5
```




```output2
902673363
```




```output3
187821763
```



## Note

<p>In the first example, there are five ways to place $2$ chips in points from $1$ to $3$ so that the cost is $1$:</p><ul> <li> $(1, 1)$; </li><li> $(1, 2)$; </li><li> $(1, 3)$; </li><li> $(2, 2)$; </li><li> $(2, 3)$. </li></ul>
