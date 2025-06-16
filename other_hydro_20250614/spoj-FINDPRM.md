<p>One commonly used method to calculate all primes in the range [2..n] is to start with the number 2, mark it as prime, and mark all its multiples (excluding itself) as not prime. Then, we find the next smallest unmarked number, mark it as prime, and mark all its multiples (excluding itself) as not prime. Continuing this way, we get a list of all primes. <br><br>Now, let us say that we modified the above algorithm, and start with n instead of 2. We mark it as prime, and mark all its factors (excluding itself) as not prime. Then we find the next greatest unmarked number, mark it as prime, and mark all its factors (excluding itself) as not prime. Continuing this way, we get a list of all primes.<br><br>Now you wonder, given a value of n, how many numbers are such that both the above algorithms will mark them as prime?</p>
<p style="text-align: center;"><br><strong>Input</strong></p>
<p><strong></strong><br>The first line contains T the number of test cases. Each of the next T lines contain an integer n.</p>
<p style="text-align: center;"><br><strong>Output</strong></p>
<p>Output T lines, one for each test case, containing the required answer.</p>
<p style="text-align: center;"><strong>Example</strong></p>
<p>Sample Input :<br>3<br>2<br>4<br>7<br><br>Sample Output :<br>1<br>1<br>2<br><br></p>
<p style="text-align: center;"><strong>Constraints</strong></p>
<p>1 &lt;= T &lt;= 100000<br>2 &lt;= n &lt;= 10000000</p>