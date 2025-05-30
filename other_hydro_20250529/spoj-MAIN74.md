<p>Consider the famous euclid algoithm to calculate the GCD of two integers (a, b):</p>
<pre>int gcd(int a, int b) {
    while (b != 0) {
        int temp = a;
        a = b;
        b = temp % b;
    }
    return a;
}</pre>

<p>for input (7, 3) the 'while' loop will run 2 times as follows: (7, 3)  =&gt; (3, 1) =&gt; (1, 0)</p>
<p>Now given an integer N you have to find the smallest possible sum of two non-negative integers a, b (a &gt;= b) such that the while loop in the above mentioned function for (a, b) will run exactly N times.</p>

<h3>Input</h3>
<p>First line of input contains T (1 &lt;= T &lt;= 50) the number of test cases. Each of the following T lines contains an integer N (0 &lt;= N &lt;= 10^18).</p>

<h3>Output</h3>
<p>For each test case print the required answer modulo 1000000007 in a seperate line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
1

<strong>Output:</strong>
2</pre>

<p>Explaination: (1,1) is the required pair.</p>