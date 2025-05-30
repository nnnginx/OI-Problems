## Description

<div><p>Squirrel Liss loves nuts. Liss asks you to plant some nut trees.</p><p>There are <span class="tex-span"><i>n</i></span> positions (numbered 1 to <span class="tex-span"><i>n</i></span> from west to east) to plant a tree along a street. Trees grow one meter per month. At the beginning of each month you should process one query. The query is one of the following types:</p><ol> <li> Plant a tree of height <span class="tex-span"><i>h</i></span> at position <span class="tex-span"><i>p</i></span>. </li><li> Cut down the <span class="tex-span"><i>x</i></span>-th existent (not cut) tree from the west (where <span class="tex-span"><i>x</i></span> is 1-indexed). When we cut the tree it drops down and takes all the available place at the position where it has stood. So no tree can be planted at this position anymore. </li></ol><p>After processing each query, you should print the length of the longest increasing subsequence. A subset of existent trees is called an <span class="tex-font-style-it">increasing subsequence</span> if the height of the trees in the set is strictly increasing from west to east (for example, the westmost tree in the set must be the shortest in the set). The length of the increasing subsequence is the number of trees in it.</p><p>Note that Liss don't like the trees with the same heights, so it is guaranteed that at any time no two trees have the exactly same heights.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1  ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of positions and the number of queries.</p><p>Next <span class="tex-span"><i>m</i></span> lines contains the information of queries by following formats:</p><ul> <li> If the <span class="tex-span"><i>i</i></span>-th query is type 1, the <span class="tex-span"><i>i</i></span>-th line contains three integers: 1, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the position of the new tree and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the initial height of the new tree. </li><li> If the <span class="tex-span"><i>i</i></span>-th query is type 2, the <span class="tex-span"><i>i</i></span>-th line contains two integers: 2 and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>), where the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the index of the tree we want to cut. </li></ul><p>The input is guaranteed to be correct, i.e.,</p><ul> <li> For type 1 queries, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> will be pairwise distinct. </li><li> For type 2 queries, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will be less than or equal to the current number of trees. </li><li> At any time no two trees have the exactly same heights. </li></ul><p>In each line integers are separated by single spaces.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the length of the longest increasing subsequence after each query. Separate the numbers by whitespaces.</p></div>


## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1  ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of positions and the number of queries.</p><p>Next <span class="tex-span"><i>m</i></span> lines contains the information of queries by following formats:</p><ul> <li> If the <span class="tex-span"><i>i</i></span>-th query is type 1, the <span class="tex-span"><i>i</i></span>-th line contains three integers: 1, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the position of the new tree and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the initial height of the new tree. </li><li> If the <span class="tex-span"><i>i</i></span>-th query is type 2, the <span class="tex-span"><i>i</i></span>-th line contains two integers: 2 and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>), where the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the index of the tree we want to cut. </li></ul><p>The input is guaranteed to be correct, i.e.,</p><ul> <li> For type 1 queries, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> will be pairwise distinct. </li><li> For type 2 queries, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will be less than or equal to the current number of trees. </li><li> At any time no two trees have the exactly same heights. </li></ul><p>In each line integers are separated by single spaces.</p>


## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the length of the longest increasing subsequence after each query. Separate the numbers by whitespaces.</p>


## Samples

```input1
4 6
1 1 1
1 4 4
1 3 4
2 2
1 2 8
2 3

```

```output1
1
2
3
2
2
2

```




## Note

<p>States of street after each query you can see on the following animation:</p><center> <img class="tex-graphics" src="./26289/file/rGp5y883.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If your browser doesn't support animation png, please see the gif version here: http://212.193.37.254/codeforces/images/162/roadtree.gif</p>

