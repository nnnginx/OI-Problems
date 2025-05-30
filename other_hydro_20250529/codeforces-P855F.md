## Description

<div><p>Nagini, being a horcrux You-know-who created with the murder of Bertha Jorkins, has accumulated its army of snakes and is launching an attack on Hogwarts school. </p><p>Hogwarts' entrance can be imagined as a straight line (x-axis) from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>. Nagini is launching various snakes at the Hogwarts entrance. Each snake lands parallel to the entrance, covering a segment at a distance <span class="tex-span"><i>k</i></span> from <span class="tex-span"><i>x</i> = <i>l</i></span> to <span class="tex-span"><i>x</i> = <i>r</i></span>. Formally, each snake can be imagined as being a line segment between points <span class="tex-span">(<i>l</i>, <i>k</i>)</span> and <span class="tex-span">(<i>r</i>, <i>k</i>)</span>. Note that <span class="tex-span"><i>k</i></span> can be both positive and negative, but not <span class="tex-span">0</span>.</p><p>Let, at some <span class="tex-span"><i>x</i></span>-coordinate <span class="tex-span"><i>x</i> = <i>i</i></span>, there be snakes at point <span class="tex-span">(<i>i</i>, <i>y</i><sub class="lower-index">1</sub>)</span> and point <span class="tex-span">(<i>i</i>, <i>y</i><sub class="lower-index">2</sub>)</span>, such that <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> &gt; 0</span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub> &lt; 0</span>. Then, if for any point <span class="tex-span">(<i>i</i>, <i>y</i><sub class="lower-index">3</sub>)</span> containing a snake such that <span class="tex-span"><i>y</i><sub class="lower-index">3</sub> &gt; 0</span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">3</sub></span> holds and for any point <span class="tex-span">(<i>i</i>, <i>y</i><sub class="lower-index">4</sub>)</span> containing a snake such that <span class="tex-span"><i>y</i><sub class="lower-index">4</sub> &lt; 0</span>, <span class="tex-span">|<i>y</i><sub class="lower-index">2</sub>| ≤ |<i>y</i><sub class="lower-index">4</sub>|</span> holds, then the danger value at coordinate <span class="tex-span"><i>x</i> = <i>i</i></span> is <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> + |<i>y</i><sub class="lower-index">2</sub>|</span>. If no such <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> exist, danger value is <span class="tex-span">0</span>. </p><p>Harry wants to calculate the danger value of various segments of the Hogwarts entrance. Danger value for a segment <span class="tex-span">[<i>l</i>, <i>r</i>)</span> of the entrance can be calculated by taking the sum of danger values for each integer <span class="tex-span"><i>x</i></span>-coordinate present in the segment.</p><p>Formally, you have to implement two types of queries:</p><ul> <li> <span class="tex-font-style-tt">1 l r k</span>: a snake is added parallel to entrance from <span class="tex-span"><i>x</i> = <i>l</i></span> to <span class="tex-span"><i>x</i> = <i>r</i></span> at y-coordinate <span class="tex-span"><i>y</i> = <i>k</i></span> (<span class="tex-span"><i>l</i></span> inclusive, <span class="tex-span"><i>r</i></span> exclusive). </li><li> <span class="tex-font-style-tt">2 l r</span>: you have to calculate the danger value of segment <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (<span class="tex-span"><i>l</i></span> inclusive, <span class="tex-span"><i>r</i></span> exclusive). </li></ul></div><div class="input-specification"><p>First line of input contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">4</sup></span>) denoting the number of queries.</p><p>Next <span class="tex-span"><i>q</i></span> lines each describe a query. Each query description first contains the query type <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>). This is followed by further description of the query. In case of the type being <span class="tex-span">1</span>, it is followed by integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="./28755/file/awk7i42d.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>k</i> ≠ 0</span>). Otherwise, it just contains two integers, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Output the answer for each query of type 2 in a separate line.</p></div>

## Input

<p>First line of input contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">4</sup></span>) denoting the number of queries.</p><p>Next <span class="tex-span"><i>q</i></span> lines each describe a query. Each query description first contains the query type <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>). This is followed by further description of the query. In case of the type being <span class="tex-span">1</span>, it is followed by integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="./28755/file/awk7i42d.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>k</i> ≠ 0</span>). Otherwise, it just contains two integers, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Output the answer for each query of type 2 in a separate line.</p>

## Samples

```input1
3
1 1 10 10
1 2 4 -7
2 1 10

```

```output1
34

```






```input2
7
1 2 3 5
1 1 10 10
1 4 5 -5
2 4 8
1 1 10 -10
2 4 8
2 1 10

```

```output2
15
75
170

```




## Note

<p>In the first sample case, the danger value for <span class="tex-span"><i>x</i></span>-coordinates <span class="tex-span">1</span> is <span class="tex-span">0</span> as there is no <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> satisfying the above condition for <span class="tex-span"><i>x</i> = 1</span>.</p><p>Danger values for <span class="tex-span"><i>x</i></span>-coordinates <span class="tex-span">2</span> and <span class="tex-span">3</span> is <span class="tex-span">10 + | - 7| = 17</span>.</p><p>Danger values for <span class="tex-span"><i>x</i></span>-coordinates <span class="tex-span">4</span> to <span class="tex-span">9</span> is again <span class="tex-span">0</span> as there is no <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> satisfying the above condition for these coordinates.</p><p>Thus, total danger value is <span class="tex-span">17 + 17 = 34</span>.</p>
