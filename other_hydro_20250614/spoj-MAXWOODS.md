<p><strong>Problem Statement:</strong></p>
<p><img src="../../../content/cegprakash:maxwoods.png" alt="" width="821" height="365"></p>
<p><strong><br></strong></p>
<p>The image explains it all. You initially step at 0,0 facing right. At each step you can move according to the conditions specified in the image. You cannot step into the blocked boxes (in blue).  Find the maximum number of trees you can cut.</p>
<p><strong>Input:</strong></p>
<p>The first line consists of an integer t, the number of test cases. For each test case the first line consists of two integers m and n, the number of rows and columns. Then follows the description of the matrix M.</p>
<p>M[i][j]=¡¯T¡¯ if the region has a tree.</p>
<p>M[i][j]=¡¯#¡¯ if the region is blocked.</p>
<p>M[i][j]=¡¯0¡¯ (zero) otherwise.</p>
<p><strong>Output:</strong></p>
<p>&nbsp;</p>
<p>For each test case find the maximum trees that you can cut.</p>
<p>&nbsp;</p>
<p><strong>Input Constraints:</strong></p>
<p>1&lt;=t&lt;=10</p>
<p>1&lt;=m,n&lt;=200</p>
<p>&nbsp;</p>

<p><strong>Example:</strong></p>
<p><strong>Sample Input:</strong></p>
<pre>4
5 5
0TTTT
T#T#0
#TT#T
T00T0
T0#T0
1 1
T
3 3
T#T
TTT
T#T
1 1
#</pre>

<p><strong>Sample Output:</strong></p>
<pre>8
1
3
0</pre>

<p><strong>Solution for test case #1:</strong></p>
<p><img src="./23311/file/3xxF8oxM.png" alt="" width="350" height="350"></p>