## Description

<div><p>Every airport has a baggage claim area, and Balbesovo Airport is no exception. At some point, one of the administrators at Sheremetyevo came up with an unusual idea: to change the traditional shape of the baggage claim conveyor from a carousel to a more complex form.</p><p>Suppose that the baggage claim area is represented as a rectangular grid of size $n \times m$. The administration proposed that the path of the conveyor should pass through the cells $p_1, p_2, \ldots, p_{2k+1}$, where $p_i = (x_i, y_i)$.</p><p>For each cell $p_i$ and the next cell $p_{i+1}$ (where $1 \leq i \leq 2k$), these cells must share a common side. Additionally, the path must be simple, meaning that for no pair of indices $i \neq j$ should the cells $p_i$ and $p_j$ coincide.</p><p>Unfortunately, the route plan was accidentally spoiled by spilled coffee, and only the cells with odd indices of the path were preserved: $p_1, p_3, p_5, \ldots, p_{2k+1}$. Your task is to determine the number of ways to restore the original complete path $p_1, p_2, \ldots, p_{2k+1}$ given these $k+1$ cells.</p><p>Since the answer can be very large, output it modulo $10^9+7$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 3 \cdot 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($1 \le n, m \le 1000$, $n \cdot m \ge 3$, $1 \le k \le \left\lfloor \frac12 (n m - 1) \right\rfloor$) �� the dimensions of the grid and a parameter defining the length of the path.</p><p>Next, there are $k+1$ lines, the $i$-th of which contains two integers $x_{2i-1}$ and $y_{2i-1}$ ($1 \le x_{2i-1} \le n$, $1 \le y_{2i-1} \le m$) �� the coordinates of the cell $p_{2i-1}$ that lies on the path.</p><p>It is guaranteed that all pairs $(x_{2i-1}, y_{2i-1})$ are distinct.</p><p>It is guaranteed that the sum $n \cdot m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the number of ways to restore the original complete path modulo $10^9+7$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 3 \cdot 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($1 \le n, m \le 1000$, $n \cdot m \ge 3$, $1 \le k \le \left\lfloor \frac12 (n m - 1) \right\rfloor$) �� the dimensions of the grid and a parameter defining the length of the path.</p><p>Next, there are $k+1$ lines, the $i$-th of which contains two integers $x_{2i-1}$ and $y_{2i-1}$ ($1 \le x_{2i-1} \le n$, $1 \le y_{2i-1} \le m$) �� the coordinates of the cell $p_{2i-1}$ that lies on the path.</p><p>It is guaranteed that all pairs $(x_{2i-1}, y_{2i-1})$ are distinct.</p><p>It is guaranteed that the sum $n \cdot m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer �� the number of ways to restore the original complete path modulo $10^9+7$.</p>





```input1|2,3,4,5,9,10,11,12,13,14,15,16,17,18,19,20,21,28,29,30,31
5
2 4 2
1 1
2 2
2 4
1 4 1
1 1
1 4
5 5 11
2 5
3 4
4 5
5 4
4 3
5 2
4 1
3 2
2 1
1 2
2 3
1 4
3 4 4
1 2
2 1
3 2
2 3
3 4
3 3 2
2 2
1 1
1 3
```




```output1
2
0
2
5
1
```



## Note

<p>In the first test case, there are two possible paths:</p><ul> <li> $(1,1) \to (2,1) \to (2, 2) \to (2, 3) \to (2, 4)$ </li><li> $(1,1) \to (1,2) \to (2, 2) \to (2, 3) \to (2, 4)$ </li></ul><p>In the second test case, there is no suitable path, as the cells $(1,1)$ and $(1,4)$ do not have a common neighboring cell.</p>
