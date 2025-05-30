## Description

<div><p>You've got a <span class="tex-span">5 × 5</span> matrix, consisting of <span class="tex-span">24</span> zeroes and a single number one. Let's index the matrix rows by numbers from <span class="tex-span">1</span> to <span class="tex-span">5</span> from top to bottom, let's index the matrix columns by numbers from <span class="tex-span">1</span> to <span class="tex-span">5</span> from left to right. In one move, you are allowed to apply one of the two following transformations to the matrix:</p><ol> <li> Swap two neighboring matrix rows, that is, rows with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> for some integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; 5)</span>. </li><li> Swap two neighboring matrix columns, that is, columns with indexes <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>j</i> + 1</span> for some integer <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>j</i> &lt; 5)</span>. </li></ol><p>You think that a matrix looks <span class="tex-font-style-it">beautiful</span>, if the single number one of the matrix is located in its middle (in the cell that is on the intersection of the third row and the third column). Count the minimum number of moves needed to make the matrix beautiful.</p></div><div class="input-specification"><p>The input consists of five lines, each line contains five integers: the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line of the input represents the element of the matrix that is located on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column. It is guaranteed that the matrix consists of <span class="tex-span">24</span> zeroes and a single number one.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of moves needed to make the matrix beautiful.</p></div>


## Input

<p>The input consists of five lines, each line contains five integers: the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line of the input represents the element of the matrix that is located on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column. It is guaranteed that the matrix consists of <span class="tex-span">24</span> zeroes and a single number one.</p>


## Output

<p>Print a single integer — the minimum number of moves needed to make the matrix beautiful.</p>


## Samples

```input1
0 0 0 0 0
0 0 0 0 1
0 0 0 0 0
0 0 0 0 0
0 0 0 0 0

```

```output1
3

```






```input2
0 0 0 0 0
0 0 0 0 0
0 1 0 0 0
0 0 0 0 0
0 0 0 0 0

```

```output2
1

```



