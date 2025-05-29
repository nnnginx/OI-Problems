<p>
Bhelu is the classmate of Bablu who made the <a href="https://www.spoj.com/problems/APS/" target="next"> Amazing Prime Sequence </a>.
</p>
<p>
He felt jealous of his classmate and decides to make his own sequence. Since he was not very imaginative, he came up with almost the same definition just making a difference in f(n):
</p>
<ul>
  <li>a[0] = a[1] = 0.</li>
  <li>For n &gt; 1, a[n] = a[n - 1] + f(n), where f(n) is the sum of positive integers in the following set S.</li>
  <li>S = {x | x &lt; n and n % x = 0}.</li>
</ul>

<p>
Now, Bablu asked him to make a code to find f(n) as he already had the code of his sequence. So, Bhelu asks for your help since he doesn't know Programming. Your task is very simple, just find a[n] for a given value of n (&lt; 10^6).
</p>

<h3>Input</h3>
<p>Your code will be checked for multiple Test Cases.</p>
<p>First Line of Input contains T (&lt;= 100), the number of Test Cases.</p>
<p>Next T lines contain a single positive integer N. (1 &lt; N &lt; 10^6).</p>

<h3>Output</h3>
<p>Single line containing a[n] i.e. n-th number of the sequence for each test case.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
3
4
5

<strong>Output:</strong>
2
5
6</pre>

<p><strong>Explanation</strong></p>
<pre>f(2) = 1 {1}
f(3) = 1 {1}
f(4) = 3 {1, 2}
f(5) = 1 {1}</pre>