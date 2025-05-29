<p><span style="font-size: medium;">One day while chilling in college, Deepankar and Rishabh were discussing some extremely complex topics which are beyond the comprehension of normal people. Just then, Amit meets up with them and listens in to what they have to say. It turns out they were discussing a problem. Though (as expected) , the problem blew Amit's mind. He had no clue what to do with it or how to go about it. So it's up to you to help Amit in solving this problem.</span></p>
<p><strong><span style="font-size: medium;">Problem Statement<br></span></strong></p>
<p><span style="font-size: medium;">You are initially given a single node ( numbered as 1 ) having a value of 0. Now you will be given queries of the following types :<br><br>1. <strong>ADD</strong> : Add a new node to the graph having some integer value , by making an edge from a pre-existing node to this node.<br>2. <strong>RETURN</strong> : Return the net value added to a subtree rooted at a node X between time A and B ( inclusive ) .<br><br>The initial node is considered the root of the tree that is formed.<br><br>Each ADD query will take 1 time unit while each RETURN query will take 0 time.<br>The clock will start from time 1, i.e the current time before all queries is 1 , after first ADD it will be 2 and so on.<br><br>The number of any node inserted into the graph is based on the order the nodes were put in the graph. The initial node is 1, the next inserted node is 2 , the next is 3 and so on.<br><br>The value of any node inserted into the graph is V + answer for previous RETURN query, where V is given in ADD query. If no RETURN queries have been done yet then we take only value of V as value of node.<br><br>Since the net value may become large , print the answer to each query as the remainder on its division by <strong>1000000007</strong>.</span></p>
<h3>Input</h3>
<p><span style="font-size: medium;">The first line contains a single integer <strong>Q</strong> ,&nbsp; denoting the number of queries.</span></p>
<p><span style="font-size: medium;">The remaining lines represent each query. The first number in each query line denotes the type of query , <strong>1</strong> for <strong>ADD</strong> and <strong>2</strong> for <strong>RETURN</strong>. In case of an <strong>ADD</strong> query you will have 2 more numbers in the line , <strong>X</strong> and <strong>V</strong> , where <strong>X</strong> is the number of the node to which the current node is joined and meaning of <strong>V</strong> is as mentioned in the problem statement. In case of a <strong>RETURN</strong> query you will have 3 more numbers in the line , <strong>A</strong> ,<strong>B</strong> and <strong>X</strong> , where their meaning is as defined in the problem statement.</span></p>
<p><span style="font-size: medium;">It can be assumed that for an <strong>ADD</strong> query node <strong>X</strong> will always be a node which exists in the graph.</span></p>
<h3>Output</h3>
<p><span style="font-size: medium;">For each <strong>RETURN</strong> query output a single line containing the answer for that query.</span></p>
<h3>Constraints</h3>
<p><span style="font-size: medium;">1 &lt;= <strong>Q</strong> &lt;= 200000</span></p>
<p><span style="font-size: medium;">0 &lt;= <strong>V</strong> &lt;= 1000000000</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>1 1 10<br>2 1 2 1<br>1 1 5

<strong>Output:</strong>
10
</pre>