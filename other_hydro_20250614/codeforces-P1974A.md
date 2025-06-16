## Description

<div><p>Little Rosie has a phone with a desktop (or launcher, as it is also called). The desktop can consist of several screens. Each screen is represented as a grid of size $5 \times 3$, i.e., five rows and three columns.</p><p>There are $x$ applications with an icon size of $1 \times 1$ cells; such an icon occupies only one cell of the screen. There are also $y$ applications with an icon size of $2 \times 2$ cells; such an icon occupies a <span class="tex-font-style-bf">square</span> of $4$ cells on the screen. Each cell of each screen can be occupied by no more than one icon.</p><p>Rosie wants to place the application icons on the minimum number of screens. Help her find the minimum number of screens needed.</p></div><div class="input-specification"><p>The first line of the input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. </p><p>The first and only line of each test case contains two integers $x$ and $y$ ($0 \leq x, y \leq 99$)&nbsp;！ the number of applications with a $1 \times 1$ icon and the number of applications with a $2 \times 2$ icon, respectively.</p></div><div class="output-specification"><p>For each test case, output the minimal number of required screens on a separate line.</p></div>

## Input

<p>The first line of the input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. </p><p>The first and only line of each test case contains two integers $x$ and $y$ ($0 \leq x, y \leq 99$)&nbsp;！ the number of applications with a $1 \times 1$ icon and the number of applications with a $2 \times 2$ icon, respectively.</p>

## Output

<p>For each test case, output the minimal number of required screens on a separate line.</p>





```input1|2,4,6,8,10,12
11
1 1
7 2
12 4
0 3
1 0
8 1
0 0
2 0
15 0
8 2
0 9
```




```output1
1
1
2
2
1
1
0
1
1
2
5
```



## Note

<p>The solution for the first test case can look as follows:</p><center> <img class="tex-graphics" height="189px" src="./34668/file/fmu8HNjs.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Blue squares represent empty spaces for icons, green squares represent $1 \times 1$ icons, red squares represent $2 \times 2$ icons</span> </center><p>The solution for the third test case can look as follows:</p><center> <img class="tex-graphics" height="189px" src="./34668/file/gsfKnomA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
