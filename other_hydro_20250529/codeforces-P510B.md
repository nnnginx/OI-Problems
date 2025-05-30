## Description

<div><p>Fox Ciel is playing a mobile puzzle game called "Two Dots". The basic levels are played on a board of size <span class="tex-span"><i>n</i> × <i>m</i></span> cells, like this:</p><center><img class="tex-graphics" src="./27273/file/EKflsb4L.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Each cell contains a dot that has some color. We will use different uppercase Latin characters to express different colors.</p><p>The key of this game is to find a cycle that contain dots of same color. Consider 4 blue dots on the picture forming a circle as an example. Formally, we call a sequence of dots <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>k</i></sub></span> a <span class="tex-font-style-underline">cycle</span> if and only if it meets the following condition:</p><ol> <li> These <span class="tex-span"><i>k</i></span> dots are different: if <span class="tex-span"><i>i</i> ≠ <i>j</i></span> then <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is different from <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span>. </li><li> <span class="tex-span"><i>k</i></span> is at least 4. </li><li> All dots belong to the same color. </li><li> For all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i> - 1</span>: <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i> + 1</sub></span> are adjacent. Also, <span class="tex-span"><i>d</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> should also be adjacent. Cells <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are called adjacent if they share an edge. </li></ol><p>Determine if there exists a <span class="tex-font-style-underline">cycle</span> on the field.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 50</span>): the number of rows and columns of the board.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains a string consisting of <span class="tex-span"><i>m</i></span> characters, expressing colors of dots in each line. Each character is an uppercase Latin letter.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Yes</span>" if there exists a <span class="tex-font-style-underline">cycle</span>, and "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 50</span>): the number of rows and columns of the board.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains a string consisting of <span class="tex-span"><i>m</i></span> characters, expressing colors of dots in each line. Each character is an uppercase Latin letter.</p>


## Output

<p>Output "<span class="tex-font-style-tt">Yes</span>" if there exists a <span class="tex-font-style-underline">cycle</span>, and "<span class="tex-font-style-tt">No</span>" otherwise.</p>


## Samples

```input1
3 4
AAAA
ABCA
AAAA

```

```output1
Yes

```






```input2
3 4
AAAA
ABCA
AADA

```

```output2
No

```






```input3
4 4
YYYR
BYBY
BBBY
BBBY

```

```output3
Yes

```






```input4
7 6
AAAAAB
ABBBAB
ABAAAB
ABABBB
ABAAAB
ABBBAB
AAAAAB

```

```output4
Yes

```






```input5
2 13
ABCDEFGHIJKLM
NOPQRSTUVWXYZ

```

```output5
No

```




## Note

<p>In first sample test all '<span class="tex-font-style-tt">A</span>' form a cycle.</p><p>In second sample there is no such cycle.</p><p>The third sample is displayed on the picture above ('<span class="tex-font-style-tt">Y</span>' = Yellow, '<span class="tex-font-style-tt">B</span>' = Blue, '<span class="tex-font-style-tt">R</span>' = Red).</p>

