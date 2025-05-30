## Description

<div><p>The teacher gave Anton a large geometry homework, but he didn't do it (as usual) as he participated in a regular round on Codeforces. In the task he was given a set of <span class="tex-span"><i>n</i></span> lines defined by the equations <span class="tex-span"><i>y</i> = <i>k</i><sub class="lower-index"><i>i</i></sub>·<i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub></span>. It was necessary to determine whether there is at least one point of intersection of two of these lines, that lays strictly inside the strip between <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub></span>. In other words, is it true that there are <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span> and <span class="tex-span"><i>x</i>', <i>y</i>'</span>, such that: </p><ul> <li> <span class="tex-span"><i>y</i>' = <i>k</i><sub class="lower-index"><i>i</i></sub> * <i>x</i>' + <i>b</i><sub class="lower-index"><i>i</i></sub></span>, that is, point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> belongs to the line number <span class="tex-span"><i>i</i></span>; </li><li> <span class="tex-span"><i>y</i>' = <i>k</i><sub class="lower-index"><i>j</i></sub> * <i>x</i>' + <i>b</i><sub class="lower-index"><i>j</i></sub></span>, that is, point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> belongs to the line number <span class="tex-span"><i>j</i></span>; </li><li> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i>' &lt; <i>x</i><sub class="lower-index">2</sub></span>, that is, point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> lies inside the strip bounded by <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub></span>. </li></ul><p>You can't leave Anton in trouble, can you? Write a program that solves the given task.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of lines in the task given to Anton. The second line contains integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 1 000 000 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 1 000 000</span>) defining the strip inside which you need to find a point of intersection of at least two lines.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1 000 000 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the descriptions of the lines. It is guaranteed that all lines are pairwise distinct, that is, for any two <span class="tex-span"><i>i</i> ≠ <i>j</i></span> it is true that either <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> ≠ <i>k</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes), if there is at least one intersection of two distinct lines, located strictly inside the strip. Otherwise print "<span class="tex-font-style-tt">No</span>" (without quotes).</p></div>


## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of lines in the task given to Anton. The second line contains integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 1 000 000 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 1 000 000</span>) defining the strip inside which you need to find a point of intersection of at least two lines.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1 000 000 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the descriptions of the lines. It is guaranteed that all lines are pairwise distinct, that is, for any two <span class="tex-span"><i>i</i> ≠ <i>j</i></span> it is true that either <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> ≠ <i>k</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p>


## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes), if there is at least one intersection of two distinct lines, located strictly inside the strip. Otherwise print "<span class="tex-font-style-tt">No</span>" (without quotes).</p>


## Samples

```input1
4
1 2
1 2
1 0
0 1
0 2

```

```output1
NO
```






```input2
2
1 3
1 0
-1 3

```

```output2
YES
```






```input3
2
1 3
1 0
0 2

```

```output3
YES
```






```input4
2
1 3
1 0
0 3

```

```output4
NO
```




## Note

<p>In the first sample there are intersections located on the border of the strip, but there are no intersections located strictly inside it.</p><center> <img class="tex-graphics" src="./27599/file/3O5HDZ9M.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>

