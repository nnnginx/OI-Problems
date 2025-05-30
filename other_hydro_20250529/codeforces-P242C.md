## Description

<div><p>The black king is standing on a chess field consisting of <span class="tex-span">10<sup class="upper-index">9</sup></span> rows and <span class="tex-span">10<sup class="upper-index">9</sup></span> columns. We will consider the rows of the field numbered with integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> from top to bottom. The columns are similarly numbered with integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> from left to right. We will denote a cell of the field that is located in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p><p>You know that some squares of the given chess field are <span class="tex-font-style-it">allowed</span>. All allowed cells of the chess field are given as <span class="tex-span"><i>n</i></span> segments. Each segment is described by three integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting that cells in columns from number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive in the <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th row are allowed.</p><p>Your task is to find the minimum number of moves the king needs to get from square <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span> to square <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, provided that he only moves along the allowed cells. In other words, the king can be located only on allowed cells on his way.</p><p>Let us remind you that a chess king can move to any of the neighboring cells in one move. Two cells of a chess field are considered neighboring if they share at least one point.</p></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">9</sup>)</span>, denoting the initial and the final positions of the king.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, denoting the number of segments of allowed cells. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of these segments. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting that cells in columns from number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive in the <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th row are allowed. Note that the segments of the allowed cells can intersect and embed arbitrarily.</p><p>It is guaranteed that the king's initial and final position are allowed cells. It is guaranteed that the king's initial and the final positions do not coincide. It is guaranteed that the total length of all given segments doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>If there is no path between the initial and final position along allowed cells, print -1.</p><p>Otherwise print a single integer — the minimum number of moves the king needs to get from the initial position to the final one.</p></div>


## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">9</sup>)</span>, denoting the initial and the final positions of the king.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, denoting the number of segments of allowed cells. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of these segments. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting that cells in columns from number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive in the <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th row are allowed. Note that the segments of the allowed cells can intersect and embed arbitrarily.</p><p>It is guaranteed that the king's initial and final position are allowed cells. It is guaranteed that the king's initial and the final positions do not coincide. It is guaranteed that the total length of all given segments doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>


## Output

<p>If there is no path between the initial and final position along allowed cells, print -1.</p><p>Otherwise print a single integer — the minimum number of moves the king needs to get from the initial position to the final one.</p>


## Samples

```input1
5 7 6 11
3
5 3 8
6 7 11
5 2 5

```

```output1
4

```






```input2
3 4 3 10
3
3 1 4
4 5 9
3 10 10

```

```output2
6

```






```input3
1 1 2 10
2
1 1 3
2 6 10

```

```output3
-1

```



