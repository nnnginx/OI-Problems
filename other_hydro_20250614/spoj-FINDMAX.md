<p>
One way of finding the maximum element in an array is to initialize a variable to the first element in the array, iterate through the remaining array, and update the variable whenever a value strictly greater than it is found. Assuming that the array contains N elements each in the range 1..K, how many such arrays exist such that the above algorithm performs exactly P updates? Initialization of the variable is not counted as an update.
</p>

<p>
For example,the possible arrays for N = 4, K = 3 and P = 2 are:<br>
1) {1,1,2,3}<br>2) {1,2,1,3}<br>3) {1,2,2,3}<br>4) {1,2,3,1}<br>5) {1,2,3,2}<br>6) {1,2,3,3}</p>

<h3>Input</h3>
<p>
The first line contains T the number of test cases. There follow T lines, containing 3 space seperated integers N, K and P.
</p>

<h3>Output</h3>
<p>
Output T lines, one for each test case. On each line, output the answer as asked above. Since the answers can get very big, output the answer modulo 1000000007.</p>

<h3>Example</h3>
<pre><b>Sample Input:</b>
3
4 3 2
2 3 1
3 4 1

<b>Sample Output:</b>
6
3
30</pre>

<h3>Constraints</h3>
<p>
1 &lt;= T &lt;= 100<br>
1 &lt;= n &lt;= 100<br>
1 &lt;= K &lt;= 300<br>
0 &lt;= P &lt; n
</p>