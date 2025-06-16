<p>Mahesh and Ramashish are good friends. Each day Ramashish gives an array arr[0,1,2...,n-1] of size 'n' to Mahesh and asks him to modify it.<br>Modifying an array means to execute the following operation exactly 'k' times:
</p><ul>
  <li>"Replace any array element 'x' by '-x' i.e multiply it by -1."</li>
</ul>
<p></p>

<p>
Note that this operation can be performed on an array element zero,one or more times. But while modifying the array, Mahesh should also keep in mind that the sum of the elements of the final array should be <b>maximum possible</b>. Mahesh wants to go to sleep so he has to finish this job as soon as possible. Can you help him? </p>

<h3>Input</h3>
<p>First line of the input contains the number of test cases 'T'. Then follow 2T lines describing the test cases(Two lines for every test case).</p>
<p>For each test case, First line has two space separated integers  'n' (Number of elements in the array) and 'k' (Number of times to execute the operation described above) and the next line has 'n' space separated integers in non-decreasing order which are the array elements.</p>

<h3>Constraints</h3>
<ul>
  <li>1 &lt;= T &lt;=10</li>
  <li>1 &lt;= n &lt;= 100</li>
  <li>1 &lt;= k &lt;= 100</li>
</ul>
<p>For each 0 &lt;= i &lt;= n-1, -10^5 &lt;= arr[i] &lt;= 10^5.</p> 

<h3>Output</h3>
<p>Output T lines, one for each test case denoting the maximum possible sum which can be obtained after modifying the array.

</p><h3>Example</h3>
<pre><b>Input:</b>
1
3 1
-1 -1 1

<b>Output:</b>
1</pre>