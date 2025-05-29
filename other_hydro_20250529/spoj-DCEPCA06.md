<p>Alice and Bob start playing a new game. Alice writes 2 numbers - N and K. She asks Bob to find an integer which is N digits long such that the absolute difference in the adjacent digits is greater than or equal to K. Bob realizes that a lot of integers satisfy this condition. &nbsp;Can you help Bob to find the total number of N digit integers which satisfy the condition set by Alice?<br>Since the answer can be very large, print the answer modulus 1000000007.</p>
<p>Note :</p>
<p>The adjacent digits to a digit constitute both the left and right neighbor of the digit. Starting from the left, only the second digit is regarded as adjacent to the first digit and only the second last digit is regarded as adjacent to the last digit.</p>
<h3>Constraints</h3>
<p>T = 100<br> 2 &lt;= N &lt;= 10^9<br> 0 &lt;= K &lt;= 9</p>
<h3>Input</h3>
<p>First line contains T- the number of test cases. The next T lines contains two numbers N and K as given by Alice.</p>
<h3>Output</h3>
<p>Print T lines each containing the total number of integers of N digit mod 1000000007 which satisfy the condition set by Alice.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2 9<br>2 8<br>&nbsp;<br><strong>Output:</strong>
1<br>4</pre>