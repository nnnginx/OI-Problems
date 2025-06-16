<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MTREE/en/">English</a></td> 
<td width="50%"><a href="/problems/MTREE/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>As  you  are  bound  to  know  by  now,  a  tree  is  a  connected  graph consisting  of N  vertices  and N−1 edges. Trees  also  have  the  property of  there  being  exactly  a  single  unique path  between  any  pair  of 
vertices. You will be given a tree in which every edge is assigned a weight – a non negative integer. The weight of a path is the product of the weights of all edges on the path. The weight of the tree is the sum of the  weights  of  all  paths  in  the  tree.  Paths  going  in  opposite directions  (A  to  B  and  B  to  A)  are considered the same and, when calculating the weight of a tree, are counted only once.</p>

<p>Write a program that, given a tree, calculates its weight modulo 1000000007. </p>

<h3>Input</h3>
<p>The first line contains the integer N (2 ≤ N ≤ 100 000), the number of vertices in the tree. The vertices are numbered 1 to N. Each  of  the  following N−1 contains  three  integers A,  B  and W  (1 ≤ A,  B ≤ N,  0 ≤ W ≤  1000) describing one edge. The edge connects vertices A and B, and its weight is W.</p>

<h3>Output</h3>
<p>Output the weight of the tree, modulo 1000000007. </p>

<h3>Sample</h3>
<pre><b>input:</b>
3
3 2 100
2 1 100

<b>output:</b>
10200

<b>input:</b>
4
1 2 5
1 3 5
1 4 5

<b>output:</b>
90

<b>input:</b>
5
1 2 2
2 3 3
4 3 2
5 3 2

<b>output:</b>
55</pre>