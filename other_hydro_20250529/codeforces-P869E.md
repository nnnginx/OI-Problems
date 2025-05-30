## Description

<div><p><span class="tex-font-style-it">Adieu l'ami.</span></p><p>Koyomi is helping Oshino, an acquaintance of his, to take care of an open space around the abandoned Eikou Cram School building, Oshino's makeshift residence.</p><p>The space is represented by a rectangular grid of <span class="tex-span"><i>n</i> × <i>m</i></span> cells, arranged into <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. The <span class="tex-span"><i>c</i></span>-th cell in the <span class="tex-span"><i>r</i></span>-th row is denoted by <span class="tex-span">(<i>r</i>, <i>c</i>)</span>.</p><p>Oshino places and removes barriers <span class="tex-font-style-bf">around</span> rectangular areas of cells. Specifically, an action denoted by "<span class="tex-span">1 <i>r</i><sub class="lower-index">1</sub> <i>c</i><sub class="lower-index">1</sub> <i>r</i><sub class="lower-index">2</sub> <i>c</i><sub class="lower-index">2</sub></span>" means Oshino's placing barriers around a rectangle with two corners being <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span> and sides parallel to squares sides. Similarly, "<span class="tex-span">2 <i>r</i><sub class="lower-index">1</sub> <i>c</i><sub class="lower-index">1</sub> <i>r</i><sub class="lower-index">2</sub> <i>c</i><sub class="lower-index">2</sub></span>" means Oshino's removing barriers around the rectangle. <span class="tex-font-style-bf">Oshino ensures that no barriers staying on the ground share any common points, nor do they intersect with boundaries of the <span class="tex-span"><i>n</i> × <i>m</i></span> area.</span></p><p>Sometimes Koyomi tries to walk from one cell to another carefully without striding over barriers, in order to avoid damaging various items on the ground. "<span class="tex-span">3 <i>r</i><sub class="lower-index">1</sub> <i>c</i><sub class="lower-index">1</sub> <i>r</i><sub class="lower-index">2</sub> <i>c</i><sub class="lower-index">2</sub></span>" means that Koyomi tries to walk from <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span> without crossing barriers.</p><p>And you're here to tell Koyomi the feasibility of each of his attempts.</p></div><div class="input-specification"><p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2 500</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>) — the number of rows and columns in the grid, and the total number of Oshino and Koyomi's actions, respectively.</p><p>The following <span class="tex-span"><i>q</i></span> lines each describes an action, containing five space-separated integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the type and two coordinates of an action. Additionally, the following holds depending on the value of <span class="tex-span"><i>t</i></span>: </p><ul> <li> If <span class="tex-span"><i>t</i> = 1</span>: <span class="tex-span">2 ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">2 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i> - 1</span>; </li><li> If <span class="tex-span"><i>t</i> = 2</span>: <span class="tex-span">2 ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">2 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i> - 1</span>, the specified group of barriers exist on the ground before the removal. </li><li> If <span class="tex-span"><i>t</i> = 3</span>: no extra restrictions. </li></ul></div><div class="output-specification"><p>For each of Koyomi's attempts (actions with <span class="tex-span"><i>t</i> = 3</span>), output one line — containing "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it's feasible, and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2 500</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>) — the number of rows and columns in the grid, and the total number of Oshino and Koyomi's actions, respectively.</p><p>The following <span class="tex-span"><i>q</i></span> lines each describes an action, containing five space-separated integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the type and two coordinates of an action. Additionally, the following holds depending on the value of <span class="tex-span"><i>t</i></span>: </p><ul> <li> If <span class="tex-span"><i>t</i> = 1</span>: <span class="tex-span">2 ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">2 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i> - 1</span>; </li><li> If <span class="tex-span"><i>t</i> = 2</span>: <span class="tex-span">2 ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">2 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i> - 1</span>, the specified group of barriers exist on the ground before the removal. </li><li> If <span class="tex-span"><i>t</i> = 3</span>: no extra restrictions. </li></ul>

## Output

<p>For each of Koyomi's attempts (actions with <span class="tex-span"><i>t</i> = 3</span>), output one line — containing "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it's feasible, and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>

## Samples

```input1
5 6 5
1 2 2 4 5
1 3 3 3 3
3 4 4 1 1
2 2 2 4 5
3 1 1 4 4

```

```output1
No
Yes

```






```input2
2500 2500 8
1 549 1279 1263 2189
1 303 795 1888 2432
1 2227 622 2418 1161
3 771 2492 1335 1433
1 2017 2100 2408 2160
3 48 60 798 729
1 347 708 1868 792
3 1940 2080 377 1546

```

```output2
No
Yes
No

```




## Note

<p>For the first example, the situations of Koyomi's actions are illustrated below.</p><center> <img class="tex-graphics" src="./28815/file/3pGMVXbQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
