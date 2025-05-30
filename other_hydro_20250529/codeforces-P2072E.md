## Description

<div><p>Akito decided to study a new powerful spell. Since it possesses immeasurable strength, it certainly requires a lot of space and careful preparation. For this, Akito went out into the field. Let's represent the field as a Cartesian coordinate system.</p><p>For the spell, Akito needs to place $0 \le n \le 500$ staffs at <span class="tex-font-style-bf">distinct integer coordinates</span> in the field such that there will be <span class="tex-font-style-bf">exactly $k$ pairs</span> $(i, j)$ such that $1 \le i &lt; j \le n$ and $\rho(i, j) = d(i, j)$.</p><p>Here, for two points with integer coordinates $a = (x_a, y_a)$ and $b = (x_b, y_b)$, $\rho(a, b) = \sqrt{(x_a - x_b)^2 + (y_a - y_b)^2}$ and $d(a, b) = |x_a - x_b| + |y_a - y_b|$.</p></div><div class="input-specification"><p>The first line of input contains a single number $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>In the only line of each test case, there is a single number $k$ ($0 \le k \le 10^5$) ！ the number of pairs of staffs for which the equality $\rho(i, j) = d(i, j)$ must hold.</p></div><div class="output-specification"><p>For each test case, the first line of output should print the number $n$ ($0 \le n \le 500$) ！ the number of placed staffs.</p><p>In the following $n$ lines, pairs of <span class="tex-font-style-bf">integers</span> $x_i, y_i$ $(-10^9 \le x_i, y_i \le 10^9)$ should be printed ！ the coordinates of the $i$-th staff. The points in which staffs stand must be distinct.</p></div>

## Input

<p>The first line of input contains a single number $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>In the only line of each test case, there is a single number $k$ ($0 \le k \le 10^5$) ！ the number of pairs of staffs for which the equality $\rho(i, j) = d(i, j)$ must hold.</p>

## Output

<p>For each test case, the first line of output should print the number $n$ ($0 \le n \le 500$) ！ the number of placed staffs.</p><p>In the following $n$ lines, pairs of <span class="tex-font-style-bf">integers</span> $x_i, y_i$ $(-10^9 \le x_i, y_i \le 10^9)$ should be printed ！ the coordinates of the $i$-th staff. The points in which staffs stand must be distinct.</p>





```input1|2,4
3
0
2
5
```




```output1
6
69 52
4 20
789 9308706
1337 1337
-1234 -5678
23456178 707
10
-236 -346262358
273568 6435267
2365437 31441367
246574 -45642372
-236 56
4743623 -192892 
10408080 -8173135
-237415357 31441367
-78125638 278
56 143231
5
1 1
2 1
1 5
3 5
1 10
```


