## Description

<div><p>You are responsible for planning a new city! The city will be represented by a rectangular grid, where each cell is either a park or a built-up area.</p><p>The residents will naturally want to go for walks in the city parks. In particular, a <span class="tex-font-style-underline">rectangular walk</span> is a rectangle consisting of the grid cells, which is at least 2 cells long both horizontally and vertically, such that all cells on the boundary of the rectangle are parks. Note that the cells inside the rectangle can be arbitrary.</p><center> <img class="tex-graphics" src="./36061/file/yb6rQJ1G.png" style="max-width: 100.0%;max-height: 100.0%;" width="288px">  An example rectangular walk (cells with dark background). </center><p>Your favourite number is $k$. To leave a long-lasting signature, you want to design the city in such a way that it has exactly $k$ rectangular walks.</p></div><div class="input-specification"><p>The input contains a single integer $k$ ($0 \le k \le 4.194\cdot 10^{12}$).</p></div><div class="output-specification"><p>On the first line, print two integers $h$ and $w$ ($1 \le h, w \le 2025$), the height and width of the grid. On the next $h$ lines, print a string with $w$ characters each, with each character being <span class="tex-font-style-tt">#</span>, denoting a park, or <span class="tex-font-style-tt">.</span>, denoting a built-up area.</p><p>It is guaranteed that for any value of $k$ within the given limits, there exists a solution with height and width within the given limits. Any city within the given limits and with exactly $k$ rectangular walks will be accepted.</p></div>

## Input

<p>The input contains a single integer $k$ ($0 \le k \le 4.194\cdot 10^{12}$).</p>

## Output

<p>On the first line, print two integers $h$ and $w$ ($1 \le h, w \le 2025$), the height and width of the grid. On the next $h$ lines, print a string with $w$ characters each, with each character being <span class="tex-font-style-tt">#</span>, denoting a park, or <span class="tex-font-style-tt">.</span>, denoting a built-up area.</p><p>It is guaranteed that for any value of $k$ within the given limits, there exists a solution with height and width within the given limits. Any city within the given limits and with exactly $k$ rectangular walks will be accepted.</p>





```input1|
5
```




```output1
3 4
####
#.##
####
```



## Note

<p>In the <span class="tex-font-style-bf">sample</span>, here are the five possible rectangular walks:</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./36061/file/HF4mFaWR.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./36061/file/zdw90Zmm.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./36061/file/IXO63WRm.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./36061/file/EYz4JDhn.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./36061/file/8JLfffYj.png" style="max-width: 100.0%;max-height: 100.0%;" width="96px"></td></tr></tbody></table><p></p>
