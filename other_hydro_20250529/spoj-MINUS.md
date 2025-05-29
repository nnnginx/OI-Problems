<p>There are <em>n</em> integer numbers listed in one line. Every time you can arbitrarily choose two neighboring integers, kick them out and write down the result of the first number subtract the second number instead. Now, you want to get number <em>m</em> after you perform this operation <em>n-1</em> times.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them is given in the very first line.</p>
<p>For each test case:</p>
<p>The first line contains two space-separated integers <em>n</em>(1&lt;= <em>n</em> &lt;=100) and <em>m</em>(-500&lt;= <em>m</em> &lt;=500). <em>n</em> lines follow, each contains a single integer (in the range [0,100]) denotes the original numbers.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>You should output <em>n-1</em> lines, each contains a single integer p<sub>i</sub>, which denotes that you are to wipe the p<sub>i</sub>-th and (p<sub>i</sub>+1)-th number in the current sequence and use their substraction instead. Each line of your output should not have any leading or trailing white spaces.</p>
<p>You may assume that there is always a valid solution to each test case in the input file. If there are multiple solutions, any of them will be accepted.</p>
<p>Print a blank line after each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>5 4<br>12<br>10<br>4<br>3<br>5<br><br><strong>Output:</strong><br>2<br>3<br>2<br>1<br></pre>