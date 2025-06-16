<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/BRTREE/en/">English</a></td> 
<td width="50%"><a href="/problems/BRTREE/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Breadtree is a kind of tree that produces bread. At its first year, a breadtree is only a node with a bread of weight 0 on this node which is also called zeronode. Every year after that, the weight of bread on each node of the tree will increase by 1, and another branch with a zeronode will grow at the end of each node. However, there is a limit of branches on each node. That is, when the number of branches of a node reaches the limit, there won't be any more branches, but the weight of its bread will still increase. What's more, a breadtree remains unchanged when the total weight of bread is larger than 1234567890. 

</p><h3>Input</h3>
<p>There are two integers N and K on each line. N is a positive integer fit in signed 32-bit integer. K is a non-negative integer fit in signed 32-bit integer. An N equals to 0 signals the end of input, which should not be processed. 

</p><h3>Output</h3>
<p>Output the total weight of bread on a breadtree with branches limit K in the N-th year in a line for each case. 

</p><h3>Example</h3>

<pre><b>Input:</b>
10000 0
101 1
10 2
1221 128
0 0


<b>Output:</b>
9999
5050
221
2147483647

</pre>