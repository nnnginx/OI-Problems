<p>A range [L..H] is called a K-Frequent Prime range if there are atleast K primes amongst the numbers L,L+1,..,H. Given N and K, calculate how many subranges of the range [2..N] are K-Frequent Prime.<br><br></p>
<p style="text-align: center;"><strong>Input</strong></p>
<p>The first line contains the number of test cases T. Each of the next T lines contains 2 integers N and K.</p>
<p style="text-align: center;"><br><strong>Output</strong></p>
<p>Output T lines, one corresponding to each test case, containing the required answer.</p>
<p style="text-align: center;"><strong>Example</strong></p>
<p><br>Sample Input :<br>4<br>2 1<br>5 2<br>5 1<br>9 3<br><br>Sample Output :<br>1<br>4<br>9<br>8<br><br>Note : For the first test case, the only valid subrange is [2..2], whereas for the second test case, the valid subranges are : [2..3],[2..4],[2..5],[3..5].</p>
<p style="text-align: center;"><strong>Constraints</strong></p>
<p style="text-align: left;">1 &lt;= T &lt;= 100</p>
<p style="text-align: left;">2 &lt;= N &lt;= 100000</p>
<p style="text-align: left;">0 &lt;= K &lt;= 10000</p>