<p>
	The Kingdom of Byteland decided to develop a large computer network of servers 
	offering various services.
</p>
<p>
	The network is built of n servers connected by bidirectional wires. Two servers 
	can be directly connected by at most one wire. Each server can be directly 
	connected to at most 10 other servers and every two servers are connected with 
	some path in the network. Each wire has a fixed positive data transmission time 
	measured in milliseconds. The distance (in milliseconds) D(V, W) between two 
	servers V and W is defined as the length of the shortest (transmission 
	time-wise) path connecting V and W in the network. For convenience we let D(V, 
	V) = 0 for all V.
</p>
<p>
	Some servers offer more services than others. Therefore each server V is marked 
	with a natural number r(V), called a rank. The bigger the rank the more 
	powerful a server is.
</p>
<p>
	At each server, data about nearby servers should be stored. However, not all 
	servers are interesting. The data about distant servers with low ranks do not 
	have to be stored. More specifically, a server W is interesting for a server V 
	if for every server U such that D(V, U) &lt;= D(V, W) we have r(U) &lt;= r(W).
</p>
<p>
	For example, all servers of the maximal rank are interesting to all servers. If 
	a server V has the maximal rank, then exactly the servers of the maximal rank 
	are interesting for V . Let B(V) denote the set of servers interesting for a 
	server V.
</p>
<p>
	We want to compute the total amount of data about servers that need to be 
	stored in the network being the total sum of sizes of all sets B(V). The 
	Kingdom of Byteland wanted the data to be quite small so it built the network 
	in such a way that this sum does not exceed 30*n.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a server network from the standard input,
		</li><li>
		computes the total amount of data about servers that need to be stored in the 
		network,
		</li><li>
			writes the result to the standard output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer z, the number of test cases. Then z test 
	cases follow.
</p>
<p>
	For each test case, in the first line there are two natural numbers n, m, where 
	n is the number of servers in the network (1 &lt;= n &lt;= 30000) and m is the 
	number of wires (1 &lt;= m &lt;= 5n). The numbers are separated by single 
	space.
</p>
<p>
	In the next n lines the ranks of the servers are given. Line i contains one 
	integer r<sub>i</sub> (1 &lt;= r<sub>i</sub> &lt;= 10) - the rank of i-th server.
</p>
<p>
	In the following m lines the wires are described. Each wire is described by 
	three numbers a, b, t (1 &lt;= t &lt;= 1000, 1 &lt;= a, b &lt;= n, 
	a&nbsp;&lt;&gt; b), where a and b are numbers of the servers connected by the 
	wire and t is the transmission time of the wire in milliseconds.
</p>
<h3>Output</h3>
<p>
	For each test case the output consists of a single integer equal to the total 
	amount of data about servers that need to be stored in the network.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
4 3
2
3
1
1
1 4 30
2 3 20
3 4 20

<b><tt>Sample output:</tt></b>
9</pre>
<p>
	(because B(1) = {1, 2}, B(2) = {2}, B(3) = {2, 3}, B(4) = {1, 2, 3, 4})
</p>
<b>Warning: large Input/Output data, be careful with certain languages</b>