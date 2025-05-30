## Description

<div><p>Little Sofia is in fourth grade. Today in the geometry lesson she learned about segments and squares. On the way home, she decided to draw $n$ squares in the snow with a side length of $1$. For simplicity, we assume that Sofia lives on a plane and can draw only segments of length $1$, parallel to the coordinate axes, with vertices at integer points.</p><p>In order to draw a segment, Sofia proceeds as follows. If she wants to draw a vertical segment with the coordinates of the ends $(x, y)$ and $(x, y+1)$. Then Sofia looks if there is already a drawn segment with the coordinates of the ends $(x', y)$ and $(x', y+1)$ for some $x'$. If such a segment exists, then Sofia quickly draws a new segment, using the old one as a guideline. If there is no such segment, then Sofia has to take a ruler and measure a new segment for a long time. Same thing happens when Sofia wants to draw a horizontal segment, but only now she checks for the existence of a segment with the same coordinates $x$, $x+1$ and the differing coordinate $y$.</p><p>For example, if Sofia needs to draw one square, she will have to draw two segments using a ruler: </p><center> <img class="tex-graphics" src="./29855/file/UmnYeWFX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After that, she can draw the remaining two segments, using the first two as a guide: </p><center> <img class="tex-graphics" src="./29855/file/Mk9KN2kb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If Sofia needs to draw two squares, she will have to draw three segments using a ruler: </p><center> <img class="tex-graphics" src="./29855/file/KDtwUQDa.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After that, she can draw the remaining four segments, using the first three as a guide: </p><center> <img class="tex-graphics" src="./29855/file/TbqgqpjP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Sofia is in a hurry, so she wants to minimize the number of segments that she will have to draw with a ruler without a guide. Help her find this minimum number.</p></div><div class="input-specification"><p>The only line of input contains a single integer $n$ ($1 \le n \le 10^{9}$), the number of squares that Sofia wants to draw.</p></div><div class="output-specification"><p>Print single integer, the minimum number of segments that Sofia will have to draw with a ruler without a guide in order to draw $n$ squares in the manner described above.</p></div>

## Input

<p>The only line of input contains a single integer $n$ ($1 \le n \le 10^{9}$), the number of squares that Sofia wants to draw.</p>

## Output

<p>Print single integer, the minimum number of segments that Sofia will have to draw with a ruler without a guide in order to draw $n$ squares in the manner described above.</p>

## Samples

```input1
1
```

```output1
2
```






```input2
2
```

```output2
3
```






```input3
4
```

```output3
4
```



