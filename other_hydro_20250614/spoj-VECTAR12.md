<p>Mangu bought a new garden for himself. The garden is shown below in the image. The garden is semi infinite i.e. infinite in two directions (+x direction and +y direction). Garden's square cells are indexed as in the diagram. Changu comes to visit Mangu and see his garden. He is standing initially on (0,0). From a particular cell he can travel in 8 directions if possible. His task is to go from (0,0) to (n,k) in n steps. Your task is to calculate the number of possible paths he can take.</p>
<p><img src="../../../content/simes:Vectar12.png" alt="Diagram"></p>
<h3>Input</h3>
<p>The first line contains the number of test cases, T. The next T lines contain two integers n and k separated by a single space.</p>
<h3>Output</h3>
<p>You have to print the number of possible paths modulus 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1 1
2 0

<strong>Output:</strong>
1
2</pre>
<h3>Explanation</h3>
<p>The possible paths for two case are shown below:</p>
<p>Case 1:</p>
<p><img src="./24899/file/OFwMbhDr.png" alt="case1" width="320" height="240"></p>
<p>&nbsp;</p>
<p>Case 2:</p>
<p><img src="./24899/file/ezOpk5GH.png" alt="case2" width="320" height="240"></p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>T&lt;10^5</p>
<p>0&lt;=N&lt;7000</p>
<p>0&lt;=K&lt;=N</p>