<p>Penny has started taking mathematics classes and has got better at it. She now wants to challenge Sheldon at this expertise and make a fool out of him. She writes down a list of numbers as list A and calculates the median of it. The she calculates the absolute deviation of each number from this median value to make list B. Now she finds the median of this list B. She asks Sheldon to find the minimum number of elements he needs to change in list A so that the median of list B becomes equal to 0.Can you help Sheldon doing this?</p>
<p>For example :</p>
<p>List of numbers (A):&nbsp; 4 5 3 1 2 <br> Median of list A=3<br> List of Absolute Deviation from median(B) = 1 2 0 2 1<br> Median of list B = 1</p>
<p><strong>Note: Median of even length list is the mean of 2 middle values.</strong></p>
<h3>Constraints</h3>
<p>0 &lt; T &lt;= 10<br> 0 &lt; N &lt;= 10^5<br> 0 &lt;= A[i] &lt;= 10^9</p>
<h3>Input</h3>
<p>T No of testcases followed 2T lines. <br> First line of testcase contains N , size of array<br> Second line contains A[0] to A[N-1]&nbsp; the numbers of the array.</p>
<h3>Output</h3>
<p>T lines each containing a single number which denotes the minimum number of elements we need to change to get the median of the absolute deviation of numbers from median to be 0.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5<br>4 5 3 1 2<br>10<br>5 5 5 254 5 5 768 5 5 5<br><br>&nbsp;<strong>Output:</strong>
2<br>0 </pre>