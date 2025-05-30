## Description

<div><p>Koa the Koala has a matrix $A$ of $n$ rows and $m$ columns. Elements of this matrix are distinct integers from $1$ to $n \cdot m$ (each number from $1$ to $n \cdot m$ appears exactly once in the matrix).</p><p>For any matrix $M$ of $n$ rows and $m$ columns let's define the following:</p><ul> <li> The $i$-th row of $M$ is defined as $R_i(M) = [ M_{i1}, M_{i2}, \ldots, M_{im} ]$ for all $i$ ($1 \le i \le n$). </li><li> The $j$-th column of $M$ is defined as $C_j(M) = [ M_{1j}, M_{2j}, \ldots, M_{nj} ]$ for all $j$ ($1 \le j \le m$). </li></ul><p>Koa defines $S(A) = (X, Y)$ as the spectrum of $A$, where $X$ is the set of the maximum values in rows of $A$ and $Y$ is the set of the maximum values in columns of $A$.</p><p>More formally:</p><ul> <li> $X = \{ \max(R_1(A)), \max(R_2(A)), \ldots, \max(R_n(A)) \}$ </li><li> $Y = \{ \max(C_1(A)), \max(C_2(A)), \ldots, \max(C_m(A)) \}$</li></ul><p>Koa asks you to find some matrix $A'$ of $n$ rows and $m$ columns, such that each number from $1$ to $n \cdot m$ appears exactly once in the matrix, and the following conditions hold:</p><ul> <li> $S(A') = S(A)$ </li><li> $R_i(A')$ is bitonic for all $i$ ($1 \le i \le n$) </li><li> $C_j(A')$ is bitonic for all $j$ ($1 \le j \le m$) </li></ul> An array $t$ ($t_1, t_2, \ldots, t_k$) is called bitonic if it first increases and then decreases.<p> More formally: $t$ is bitonic if there exists some position $p$ ($1 \le p \le k$) such that: $t_1 &lt; t_2 &lt; \ldots &lt; t_p &gt; t_{p+1} &gt; \ldots &gt; t_k$.</p><p>Help Koa to find such matrix or to determine that it doesn't exist.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 250$) &nbsp;�� the number of rows and columns of $A$.</p><p>Each of the ollowing $n$ lines contains $m$ integers. The $j$-th integer in the $i$-th line denotes element $A_{ij}$ ($1 \le A_{ij} \le n \cdot m$) of matrix $A$. It is guaranteed that every number from $1$ to $n \cdot m$ appears exactly once among elements of the matrix.</p></div><div class="output-specification"><p>If such matrix doesn't exist, print $-1$ on a single line.</p><p>Otherwise, the output must consist of $n$ lines, each one consisting of $m$ space separated integers &nbsp;�� a description of $A'$.</p><p>The $j$-th number in the $i$-th line represents the element $A'_{ij}$.</p><p>Every integer from $1$ to $n \cdot m$ should appear exactly once in $A'$, every row and column in $A'$ must be bitonic and $S(A) = S(A')$ must hold.</p><p>If there are many answers print any.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 250$) &nbsp;�� the number of rows and columns of $A$.</p><p>Each of the ollowing $n$ lines contains $m$ integers. The $j$-th integer in the $i$-th line denotes element $A_{ij}$ ($1 \le A_{ij} \le n \cdot m$) of matrix $A$. It is guaranteed that every number from $1$ to $n \cdot m$ appears exactly once among elements of the matrix.</p>

## Output

<p>If such matrix doesn't exist, print $-1$ on a single line.</p><p>Otherwise, the output must consist of $n$ lines, each one consisting of $m$ space separated integers &nbsp;�� a description of $A'$.</p><p>The $j$-th number in the $i$-th line represents the element $A'_{ij}$.</p><p>Every integer from $1$ to $n \cdot m$ should appear exactly once in $A'$, every row and column in $A'$ must be bitonic and $S(A) = S(A')$ must hold.</p><p>If there are many answers print any.</p>

## Samples

```input1
3 3
3 5 6
1 7 9
4 8 2
```

```output1
9 5 1
7 8 2
3 6 4
```






```input2
2 2
4 1
3 2
```

```output2
4 1
3 2
```






```input3
3 4
12 10 8 6
3 4 5 7
2 11 9 1
```

```output3
12 8 6 1
10 11 9 2
3 4 5 7
```




## Note

<p>Let's analyze the first sample:</p><p>For matrix $A$ we have:</p><ul> <ul> <li> Rows: <ul> <li> $R_1(A) = [3, 5, 6]; \max(R_1(A)) = 6$ </li><li> $R_2(A) = [1, 7, 9]; \max(R_2(A)) = 9$ </li><li> $R_3(A) = [4, 8, 2]; \max(R_3(A)) = 8$ </li></ul><p> </p></li><li> Columns: <ul> <li> $C_1(A) = [3, 1, 4]; \max(C_1(A)) = 4$ </li><li> $C_2(A) = [5, 7, 8]; \max(C_2(A)) = 8$ </li><li> $C_3(A) = [6, 9, 2]; \max(C_3(A)) = 9$ </li></ul> </li></ul><p> </p><li> $X = \{ \max(R_1(A)), \max(R_2(A)), \max(R_3(A)) \} = \{ 6, 9, 8 \}$ </li><li> $Y = \{ \max(C_1(A)), \max(C_2(A)), \max(C_3(A)) \} = \{ 4, 8, 9 \}$ </li><li> So $S(A) = (X, Y) = (\{ 6, 9, 8 \}, \{ 4, 8, 9 \})$ </li></ul><p>For matrix $A'$ we have:</p><ul> <ul> <li> Rows: <ul> <li> $R_1(A') = [9, 5, 1]; \max(R_1(A')) = 9$ </li><li> $R_2(A') = [7, 8, 2]; \max(R_2(A')) = 8$ </li><li> $R_3(A') = [3, 6, 4]; \max(R_3(A')) = 6$ </li></ul><p> </p></li><li> Columns: <ul> <li> $C_1(A') = [9, 7, 3]; \max(C_1(A')) = 9$ </li><li> $C_2(A') = [5, 8, 6]; \max(C_2(A')) = 8$ </li><li> $C_3(A') = [1, 2, 4]; \max(C_3(A')) = 4$ </li></ul> </li></ul><p> </p><li> Note that each of this arrays are bitonic. </li><li> $X = \{ \max(R_1(A')), \max(R_2(A')), \max(R_3(A')) \} = \{ 9, 8, 6 \}$ </li><li> $Y = \{ \max(C_1(A')), \max(C_2(A')), \max(C_3(A')) \} = \{ 9, 8, 4 \}$ </li><li> So $S(A') = (X, Y) = (\{ 9, 8, 6 \}, \{ 9, 8, 4 \})$ </li></ul>
