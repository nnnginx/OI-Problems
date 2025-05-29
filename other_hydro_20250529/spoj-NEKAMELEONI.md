<p>"Hey! I have an awesome task with chameleons, 5 th task for Saturday’s competition."</p>
<p>"Go ahead. . . "</p>
<p>&nbsp;</p>
<p>(...)</p>
<p>“That’s too difficult, I have an easier one, they won’t even solve that one.”</p>
<p>“You are given an array of N integers from the interval [1, K]. You need to process M queries. The first</p>
<p>type of query requires you to change a number in the array to a different value, and the second type of</p>
<p>query requires you to determine the length of the shortest contiguous subarray of the current array that</p>
<p>contains all numbers from 1 to K.”</p>
<p>“Hm, I can do it in O(N^6 ). What’s the limit for N?”</p>

<h3>Input</h3>
<p>The first line of input contains the integers N, K and M (1 &lt;= N, M &lt;= 100 000, 1 &lt;= K &lt;= 50). The</p>
<p>second line of input contains N integers separated by space, the integers from the array. After that,</p>
<p>M queries follow, each in one of the following two forms:</p>
<p>• “1 p v” - change the value of the p th number into v (1 &lt;= p &lt;= N, 1 &lt;= v &lt;= K)</p>
<p>• “2” - what is the length of the shortest contiguous subarray of the array containing all the integers from 1 to K</p>

<h3>Output</h3>
<p>The output must consist of the answers to the queries of the second type, each in its own line.</p>
<p>If the required subarray doesn’t exist, output −1.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
4 3 5
2 3 1 2
2
1 3 3
2
1 1 1
2

<strong>Output:</strong>
3
-1
4</pre>