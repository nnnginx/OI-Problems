## Description

<div><p><span class="tex-font-style-it">The fundamental prerequisite for justice is not to be correct, but to be strong. That's why justice is always the victor.</span></p><p>The Cinderswarm Bee. Koyomi knows it.</p><p>The bees, according to their nature, live in a tree. To be more specific, a <span class="tex-font-style-underline">complete binary tree</span> with <span class="tex-span"><i>n</i></span> nodes numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The node numbered <span class="tex-span">1</span> is the root, and the parent of the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>) node is <img align="middle" class="tex-formula" src="./28814/file/DudZG6KD.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that, however, all edges in the tree are undirected.</p><p>Koyomi adds <span class="tex-span"><i>m</i></span> extra undirected edges to the tree, creating more complication to trick the bees. And you're here to count the number of <span class="tex-font-style-underline">simple paths</span> in the resulting graph, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. A <span class="tex-font-style-underline">simple path</span> is an alternating sequence of adjacent nodes and undirected edges, which begins and ends with nodes and does not contain any node more than once. Do note that a single node is also considered a valid <span class="tex-font-style-underline">simple path</span> under this definition. Please refer to the examples and notes below for instances.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 4</span>) — the number of nodes in the tree and the number of extra edges respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines each contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>) — describing an undirected extra edge whose endpoints are <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>Note that there may be multiple edges between nodes in the resulting graph.</p></div><div class="output-specification"><p>Output one integer — the number of <span class="tex-font-style-underline">simple paths</span> in the resulting graph, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 4</span>) — the number of nodes in the tree and the number of extra edges respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines each contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>) — describing an undirected extra edge whose endpoints are <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>Note that there may be multiple edges between nodes in the resulting graph.</p>

## Output

<p>Output one integer — the number of <span class="tex-font-style-underline">simple paths</span> in the resulting graph, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>

## Samples

```input1
3 0

```

```output1
9

```






```input2
3 1
2 3

```

```output2
15

```






```input3
2 4
1 2
2 1
1 2
2 1

```

```output3
12

```




## Note

<p>In the first example, the paths are: <span class="tex-span">(1)</span>; <span class="tex-span">(2)</span>; <span class="tex-span">(3)</span>; <span class="tex-span">(1, 2)</span>; <span class="tex-span">(2, 1)</span>; <span class="tex-span">(1, 3)</span>; <span class="tex-span">(3, 1)</span>; <span class="tex-span">(2, 1, 3)</span>; <span class="tex-span">(3, 1, 2)</span>. (For the sake of clarity, the edges between nodes are omitted since there are no multiple edges in this case.)</p><p>In the second example, the paths are: <span class="tex-span">(1)</span>; <span class="tex-span">(1, 2)</span>; <span class="tex-span">(1, 2, 3)</span>; <span class="tex-span">(1, 3)</span>; <span class="tex-span">(1, 3, 2)</span>; and similarly for paths starting with <span class="tex-span">2</span> and <span class="tex-span">3</span>. (<span class="tex-span">5 × 3 = 15</span> paths in total.)</p><p>In the third example, the paths are: <span class="tex-span">(1)</span>; <span class="tex-span">(2)</span>; any undirected edge connecting the two nodes travelled in either direction. (<span class="tex-span">2 + 5 × 2 = 12</span> paths in total.)</p>
