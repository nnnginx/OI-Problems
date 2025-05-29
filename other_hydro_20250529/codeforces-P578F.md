## Description

<div><p>You are given a box full of mirrors. Box consists of grid of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Each cell of the grid contains a mirror put in the shape of '<span class="tex-span">\</span>' or '<span class="tex-span"> / </span>' (<span class="tex-span">45</span> degree to the horizontal or vertical line). But mirrors in some cells have been destroyed. You want to put new mirrors into these grids so that the following two conditions are satisfied:</p><ol> <li> If you put a light ray horizontally/vertically into the middle of any unit segment that is side of some border cell, the light will go out from the neighboring unit segment to the segment you put the ray in.</li><li> each unit segment of the grid of the mirror box can be penetrated by at least one light ray horizontally/vertically put into the box according to the rules of the previous paragraph </li></ol><center> <img class="tex-graphics" src="./27543/file/GjFZgqvh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After you tried putting some mirrors, you find out that there are many ways of doing so. How many possible ways are there? The answer might be large, so please find the result modulo prime number <span class="tex-span"><i>MOD</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>MOD</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span">3 ≤ <i>MOD</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>, <span class="tex-span"><i>MOD</i></span> is prime), <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>n</i></span> indicates the dimensions of a box and <span class="tex-span"><i>MOD</i></span> is the number to module the answer.</p><p>The following <span class="tex-span"><i>n</i></span> lines each contains a string of length <span class="tex-span"><i>m</i></span>. Each string contains only '<span class="tex-span"> / </span>', '<span class="tex-span">\</span>', '*', where '*' denotes that the mirror in that grid has been destroyed. </p><p>It is guaranteed that the number of '*' is no more than <span class="tex-span">200</span>.</p></div><div class="output-specification"><p>Output the answer modulo <span class="tex-span"><i>MOD</i></span>.</p></div>


## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>MOD</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span">3 ≤ <i>MOD</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>, <span class="tex-span"><i>MOD</i></span> is prime), <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>n</i></span> indicates the dimensions of a box and <span class="tex-span"><i>MOD</i></span> is the number to module the answer.</p><p>The following <span class="tex-span"><i>n</i></span> lines each contains a string of length <span class="tex-span"><i>m</i></span>. Each string contains only '<span class="tex-span"> / </span>', '<span class="tex-span">\</span>', '*', where '*' denotes that the mirror in that grid has been destroyed. </p><p>It is guaranteed that the number of '*' is no more than <span class="tex-span">200</span>.</p>


## Output

<p>Output the answer modulo <span class="tex-span"><i>MOD</i></span>.</p>


## Samples

```input1
2 2 1000000007
*/
/*

```

```output1
1

```






```input2
2 2 1000000007
**
\\
```

```output2
1
```






```input3
2 2 3
**
**

```

```output3
2

```




## Note

<p>The only way for sample 1 is shown on the left picture from the statement.</p><p>The only way for sample 2 is shown on the right picture from the statement.</p><p>For the third sample, there are <span class="tex-span">5</span> possibilities that are listed below: </p><p>1.</p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/uRCu5UEc.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/EzdWrlww.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p>2.</p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/5mOIaQBz.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/KpGNEPDC.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p>3.</p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/KDBu9vAs.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/7gt5FKts.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p>4.</p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/Av2qJESI.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/2EVNiYb9.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p>5.</p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/evEJ8MEe.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p><span class="tex-font-style-tt"><img align="middle" class="tex-formula" src="./27543/file/SyrQ6KKg.png" style="max-width: 100.0%;max-height: 100.0%;"></span></p><p>The answer is then module by <span class="tex-span">3</span> so the output should be <span class="tex-span">2</span>.</p>

