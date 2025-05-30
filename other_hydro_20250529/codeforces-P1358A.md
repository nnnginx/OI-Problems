## Description

<div><p>Due to the coronavirus pandemic, city authorities obligated citizens to keep a social distance. The mayor of the city Semyon wants to light up Gluharniki park so that people could see each other even at night to keep the social distance.</p><p>The park is a rectangular table with $n$ rows and $m$ columns, where the cells of the table are squares, and the boundaries between the cells are streets. External borders are also streets. Every street has length $1$. For example, park with $n=m=2$ has $12$ streets.</p><p>You were assigned to develop a plan for lighting the park. You can put lanterns in the middle of the streets. The lamp lights two squares near it (or only one square if it stands on the border of the park).</p><center> <img class="tex-graphics" src="./31174/file/rsHCGVX5.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The park sizes are: $n=4$, $m=5$. The lighted squares are marked yellow. Please note that all streets have length $1$. Lanterns are placed in the middle of the streets. In the picture <span class="tex-font-style-bf">not all</span> the squares are lit.</span> </center><p>Semyon wants to spend the least possible amount of money on lighting but also wants people throughout the park to keep a social distance. So he asks you to find the minimum number of lanterns that are required to light all the squares.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is a line containing two integers $n$, $m$ ($1 \le n, m \le 10^4$) ！ park sizes.</p></div><div class="output-specification"><p>Print $t$ answers to the test cases. Each answer must be a single integer ！ the minimum number of lanterns that are required to light all the squares.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is a line containing two integers $n$, $m$ ($1 \le n, m \le 10^4$) ！ park sizes.</p>

## Output

<p>Print $t$ answers to the test cases. Each answer must be a single integer ！ the minimum number of lanterns that are required to light all the squares.</p>

## Samples

```input1
5
1 1
1 3
2 2
3 3
5 3
```

```output1
1
2
2
5
8
```




## Note

<p>Possible optimal arrangement of the lanterns for the $2$-nd test case of input data example: <img class="tex-graphics" src="./31174/file/KXcuJMbJ.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Possible optimal arrangement of the lanterns for the $3$-rd test case of input data example: <img class="tex-graphics" src="./31174/file/wsgCJRBX.png" style="max-width: 100.0%;max-height: 100.0%;"> </p>
