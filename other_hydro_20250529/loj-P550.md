## Description

Given a grid with $n$ rows and $m$ columns, in this grid, you can choose two different grid points and match them into a pair. Notice that a point can only be matched with no more than one point. It means unmatched points are allowed. We define a weight function $f(A, B)$ for a pair of points $A, B$ as the following form:  
$$\begin{aligned} dx &= \left|x_A - x_B\right| \\ dy &= \left|y_A - y_B\right| \\ f(A, B) &= \begin{cases} dx + dy & , dx + dy \geq k \\ 0 & , dx + dy < k \end{cases} \end{aligned}$$

The weight of a possible matching scheme is defined as the sum of weights that the matching pairs given. Your task is to calculate the maximum possible weight of all matching schemes. 

## Input Format

Read from the standard input. 

The first line contains a single integer $T$ which means the number of the test cases. 

Each of the following $T$ lines contains three integers $n, m, k$ which means the height and the width of the grid, and the constant $k$ in the weight function. 

## Output Format

Write to the standard output. 

For each test case, output a line containing a single integer ¡ª the maximum of the weight of possible matching plans. 

```input1
4
1 1 0
1 2 0
2 2 1
2 3 1
```

```output1
0
1
4
7
```

```input2
6
23 66 12
233 666 123
2333 6666 1234
23333 6666 1234
2333 66666 1234
23333 66666 12345
```

```output2
33759
34876089
34987610889
1166494448889
2682884270889
34998761108889
```

```input3
4
1 1 0
1 2 0
2 2 1
2 3 1
```

```output3
0
1
4
7
```

```input4
6
23 66 12
233 666 123
2333 6666 1234
23333 6666 1234
2333 66666 1234
23333 66666 12345
```

```output4
33759
34876089
34987610889
1166494448889
2682884270889
34998761108889
```

## Constraints

For all test cases, $1 \leq T \leq 10^5$£¬$1 \leq n,m \leq 10^6$£¬$0 \leq k \leq \min(n, m) - 1$.

Detailed constraints are as follows (blank grids denote the same constraints as mentioned above):    

|	Subtask#	|	Score (percentage)	|$T$			|	$n, m$				|	Special Constraints |
|:----------------------:|:----------------:|:-----------------------:|:-----------------------------------:|:-------------------------------------------------------------------:|
|	$1$			|	$10$		|	$\leq 20$		|	$\leq 2000$			|	$n \leq 2$								|
|	$2$			|	$15$		|	$\leq 5$		|	$\leq 8$				|	$n \times m \leq 10$ and $k = \min(n, m) - 1$	|
|	$3$			|	$25$		|	$\leq 3$		|	$\leq 16$				|	-									|
|	$4$			|	$18$		|	$\leq 100$	|	$\leq 5000$			|	$n = m$ and $n \equiv 0 \pmod 2$			|
|	$5$			|	$32$		|	$\leq 10^5$	|	$\leq 10^6$			|	-									|

