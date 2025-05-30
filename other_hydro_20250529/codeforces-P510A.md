## Description

<div><p>Fox Ciel starts to learn programming. The first task is drawing a fox! However, that turns out to be too hard for a beginner, so she decides to draw a snake instead.</p><p>A snake is a pattern on a <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>m</i></span> table. Denote <span class="tex-span"><i>c</i></span>-th cell of <span class="tex-span"><i>r</i></span>-th row as <span class="tex-span">(<i>r</i>, <i>c</i>)</span>. The tail of the snake is located at <span class="tex-span">(1, 1)</span>, then it's body extends to <span class="tex-span">(1, <i>m</i>)</span>, then goes down <span class="tex-span">2</span> rows to <span class="tex-span">(3, <i>m</i>)</span>, then goes left to <span class="tex-span">(3, 1)</span> and so on.</p><p>Your task is to draw this snake for Fox Ciel: the empty cells should be represented as dot characters ('<span class="tex-font-style-tt">.</span>') and the snake cells should be filled with number signs ('<span class="tex-font-style-tt">#</span>').</p><p>Consider sample tests in order to understand the snake pattern.</p></div><div class="input-specification"><p>The only line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 50</span>). </p><p><span class="tex-span"><i>n</i></span> is an <span class="tex-font-style-bf">odd</span> number.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines. Each line should contain a string consisting of <span class="tex-span"><i>m</i></span> characters. Do not output spaces.</p></div>


## Input

<p>The only line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 50</span>). </p><p><span class="tex-span"><i>n</i></span> is an <span class="tex-font-style-bf">odd</span> number.</p>


## Output

<p>Output <span class="tex-span"><i>n</i></span> lines. Each line should contain a string consisting of <span class="tex-span"><i>m</i></span> characters. Do not output spaces.</p>


## Samples

```input1
3 3

```

```output1
###
..#
###

```






```input2
3 4

```

```output2
####
...#
####

```






```input3
5 3

```

```output3
###
..#
###
#..
###

```






```input4
9 9

```

```output4
#########
........#
#########
#........
#########
........#
#########
#........
#########

```



