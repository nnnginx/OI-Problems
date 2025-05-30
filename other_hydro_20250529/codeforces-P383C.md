## Description

<div><p>Iahub likes trees very much. Recently he discovered an interesting tree named propagating tree. The tree consists of <span class="tex-span"><i>n</i></span> nodes numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, each node <span class="tex-span"><i>i</i></span> having an initial value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The root of the tree is node <span class="tex-span">1</span>.</p><p>This tree has a special property: when a value <span class="tex-span"><i>val</i></span> is added to a value of node <span class="tex-span"><i>i</i></span>, the value -<span class="tex-span"><i>val</i></span> is added to values of all the children of node <span class="tex-span"><i>i</i></span>. Note that when you add value -<span class="tex-span"><i>val</i></span> to a child of node <span class="tex-span"><i>i</i></span>, you also add -(-<span class="tex-span"><i>val</i></span>) to all children of the child of node <span class="tex-span"><i>i</i></span> and so on. Look an example explanation to understand better how it works.</p><p>This tree supports two types of queries:</p><ul> <li> "<span class="tex-span">1</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>val</i></span>" — <span class="tex-span"><i>val</i></span> is added to the value of node <span class="tex-span"><i>x</i></span>; </li><li> "<span class="tex-span">2</span> <span class="tex-span"><i>x</i></span>" — print the current value of node <span class="tex-span"><i>x</i></span>. </li></ul><p>In order to help Iahub understand the tree better, you must answer <span class="tex-span"><i>m</i></span> queries of the preceding type.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 200000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>. Each of the next <span class="tex-span"><i>n</i>–1</span> lines contains two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, meaning that there is an edge between nodes <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a query in the format described above. It is guaranteed that the following constraints hold for all queries: <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>val</i> ≤ 1000</span>.</p></div><div class="output-specification"><p>For each query of type two (print the value of node <span class="tex-span"><i>x</i></span>) you must print the answer to the query on a separate line. The queries must be answered in the order given in the input.</p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 200000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>. Each of the next <span class="tex-span"><i>n</i>–1</span> lines contains two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, meaning that there is an edge between nodes <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a query in the format described above. It is guaranteed that the following constraints hold for all queries: <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>val</i> ≤ 1000</span>.</p>


## Output

<p>For each query of type two (print the value of node <span class="tex-span"><i>x</i></span>) you must print the answer to the query on a separate line. The queries must be answered in the order given in the input.</p>


## Samples

```input1
5 5
1 2 1 1 2
1 2
1 3
2 4
2 5
1 2 3
1 1 2
2 1
2 2
2 4

```

```output1
3
3
0

```




## Note

<p>The values of the nodes are <span class="tex-span">[1, 2, 1, 1, 2]</span> at the beginning.</p><p>Then value <span class="tex-span">3</span> is added to node <span class="tex-span">2</span>. It propagates and value -<span class="tex-span">3</span> is added to it's sons, node <span class="tex-span">4</span> and node <span class="tex-span">5</span>. Then it cannot propagate any more. So the values of the nodes are <span class="tex-span">[1, 5, 1,  - 2,  - 1]</span>.</p><p>Then value <span class="tex-span">2</span> is added to node <span class="tex-span">1</span>. It propagates and value -<span class="tex-span">2</span> is added to it's sons, node <span class="tex-span">2</span> and node <span class="tex-span">3</span>. From node <span class="tex-span">2</span> it propagates again, adding value <span class="tex-span">2</span> to it's sons, node <span class="tex-span">4</span> and node <span class="tex-span">5</span>. Node <span class="tex-span">3</span> has no sons, so it cannot propagate from there. The values of the nodes are <span class="tex-span">[3, 3,  - 1, 0, 1]</span>.</p><p>You can see all the definitions about the tree at the following link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Tree_(graph_theory)</span></p>

