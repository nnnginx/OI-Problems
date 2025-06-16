<p>Preparing a problem set is a very hard task. There are always issues with clarity of problem statements, bugs in our solutions, input or output data, and so on. Sometimes, despite our best efforts, these issues are only found during the contest, and this can really spoil it. 

</p><p>To prevent this from happening in the future, we already started to prepare data for IPSC 2009, and we decided to use your help in doing so. Currently we are working on a simple textbook problem: "Given a weighted undirected complete graph, find its minimum spanning tree." (See the Definitions below if you are not sure what a spanning tree is.) 

</p><p>Almost everythig is already prepared for this problem: the problem statement, our solution, and also the desired output data. The only (and quite important) thing left is the input data. But creating it is not as simple as it looks. 

</p><p>The bad thing that can happen is that a graph can have more than one minimum spanning tree. If we used such a graph in the input data, we would have to write a complicated checker. And we are too lazy to do this. Therefore we want to find an input data that avoids such cases. 

</p><p>Moreover, we want the test data to be good. If all the other edges were much more expensive, the minimum spanning tree would be obvious, and many incorrect algorithms would be able to find it. Therefore we want all the edge weights to be as small as possible. </p>

<h3>Definitions</h3>

<p>A graph is a set of nodes, and a set of links. Each link connects two nodes. Each pair of nodes is connected by at most one link. Each link is assigned a positive integer (its weight). The sum of the weights of all links in a graph is the weight of that graph. 

</p><p>If every two nodes are connected by a link we say that the graph is complete. 

</p><p>A sequence of nodes v<sub>0</sub>, ¡­, v<sub>n</sub> such that for each i the nodes v<sub>i</sub> and v<sub>i+1</sub> are connected by a link, is called a path. 

</p><p>If every two nodes in a graph are connected by a path, we say that the graph is connected. 

</p><p>If there is exactly one path between any two nodes we say that graph is a tree. 

</p><p>A spanning subgraph of a connected graph G is a connected graph that contains all nodes of G and some (not necessarily all) of its links. 

</p><p>A spanning subgraph T of a graph G is called the minimum spanning tree of G if and only if no other spanning subgraph has a smaller weight. 

</p><p>Note that a given graph can have more than one spanning tree. Also note that a spanning tree is always a tree. </p>

<h3>Problem specification</h3>

<p>Given a weighted tree T, you are to find the minimum possible weight of a complete graph G such that T is the only minimum spanning tree of G.</p>

<h3>Input specification</h3>

<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line.

</p><p>First line of each test case contains an integer N(N &lt;= 15000) ¨C number of nodes in the tree. The nodes are numbered from 1 to N, inclusive. The following N - 1 lines contain a description of the tree. Each of these lines contains three integers a<sub>i</sub>, b<sub>i</sub>, w<sub>i</sub>(1&lt;= a<sub>i</sub>, b<sub>i</sub> &lt;=N, 1&lt;= w<sub>i</sub> &lt;=10000) meaning that node a<sub>i</sub> is connected with node b<sub>i</sub> by a link with weight w<sub>i</sub>.</p>


<h3>Output specification</h3>

<p>For each test case, the output shall contain one line containing one integer ¨C the minimum possible weight of a complete graph such that the given tree is its unique minimal spanning tree. </p>

<h3>Example</h3>
<pre><b>Input:</b>
2

3
1 2 4
2 3 7

4
1 2 1
1 3 1
1 4 2

<b>output:</b>
19
12
</pre>
<h3>Hint</h3>
<p>In the first test case, we have to add a link between nodes 1 and 3 with weight at least 8. 

</p><p>In the second test case, the optimal graph contains the link 2 - 3 with weight 2, and links 2 - 4 and 3 - 4 with weigths 3 each. </p>