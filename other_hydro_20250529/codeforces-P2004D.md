## Description

<div><p>There are $n$ cities located on a straight line. The cities are numbered from $1$ to $n$.</p><p>Portals are used to move between cities. There are $4$ colors of portals: blue, green, red, and yellow. Each city has portals of two different colors. You can move from city $i$ to city $j$ if they have portals of the same color (for example, you can move between a "blue-red" city and a "blue-green" city). This movement costs $|i-j|$ coins.</p><p>Your task is to answer $q$ independent queries: calculate the minimum cost to move from city $x$ to city $y$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;！ the number of cities and the number of queries, respectively.</p><p>The second line contains $n$ strings of the following types: <span class="tex-font-style-tt">BG</span>, <span class="tex-font-style-tt">BR</span>, <span class="tex-font-style-tt">BY</span>, <span class="tex-font-style-tt">GR</span>, <span class="tex-font-style-tt">GY</span>, or <span class="tex-font-style-tt">RY</span>; the $i$-th of them describes the portals located in the $i$-th city; the symbol <span class="tex-font-style-tt">B</span> indicates that there is a blue portal in the city, <span class="tex-font-style-tt">G</span>&nbsp;！ green, <span class="tex-font-style-tt">R</span>&nbsp;！ red, and <span class="tex-font-style-tt">Y</span>&nbsp;！ yellow.</p><p>The $j$-th of the next $q$ lines contains two integers $x_j$ and $y_j$ ($1 \le x_j, y_j \le n$)&nbsp;！ the description of the $j$-th query.</p><p>Additional constraints on the input: </p><ul> <li> the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$; </li><li> the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$. </li></ul></div><div class="output-specification"><p>For each query, print a single integer&nbsp;！ the minimum cost to move from city $x$ to city $y$ (or $-1$ if it is impossible).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;！ the number of cities and the number of queries, respectively.</p><p>The second line contains $n$ strings of the following types: <span class="tex-font-style-tt">BG</span>, <span class="tex-font-style-tt">BR</span>, <span class="tex-font-style-tt">BY</span>, <span class="tex-font-style-tt">GR</span>, <span class="tex-font-style-tt">GY</span>, or <span class="tex-font-style-tt">RY</span>; the $i$-th of them describes the portals located in the $i$-th city; the symbol <span class="tex-font-style-tt">B</span> indicates that there is a blue portal in the city, <span class="tex-font-style-tt">G</span>&nbsp;！ green, <span class="tex-font-style-tt">R</span>&nbsp;！ red, and <span class="tex-font-style-tt">Y</span>&nbsp;！ yellow.</p><p>The $j$-th of the next $q$ lines contains two integers $x_j$ and $y_j$ ($1 \le x_j, y_j \le n$)&nbsp;！ the description of the $j$-th query.</p><p>Additional constraints on the input: </p><ul> <li> the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$; </li><li> the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$. </li></ul>

## Output

<p>For each query, print a single integer&nbsp;！ the minimum cost to move from city $x$ to city $y$ (or $-1$ if it is impossible).</p>





```input1|2,3,4,5,6,7,8
2
4 5
BR BR GY GR
1 2
3 1
4 4
1 4
4 2
2 1
BG RY
1 2
```




```output1
1
4
0
3
2
-1
```


