<p><strong>Note:&nbsp;<br></strong><strong>If you really want to learn something by solving this problem, don't hard code!&nbsp;<br></strong><strong>There is a nice logic behind this!</strong></p>
<p>---</p>
<p>Kartheeswaran was recently reading an article on perfect numbers, whose sum of divisors equals twice the number. He was intrigued by them and decided to generate them but to his disappointment they turned out to be quite rare. So he decided to look out for a different property related to sum of divisors. What is more interesting than a number being a prime? So he decided to look out for numbers whose sum of divisors is a prime number and he was the inventor of these special numbers he gave them the name K-numbers.<br> Given a range [A,B] you are expected to find the number of K-numbers in this range.</p>
<h3>Input</h3>
<p>The first line of input indicates the number of test cases T.<br> Then in the following T lines there will be a pair of integers A and B.</p>
<h3>Output</h3>
<p>Output T lines each containing a single integer ¡®c¡¯ which denotes the number of K-numbers which lie in the interval [A,B] inclusive of the end points.<br> Constraints:<br> 1&lt;=T&lt;=10000<br> 1&lt;=A&lt;=B&lt;=10^6</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>1 5</pre>
<pre>9 10</pre>
<pre><strong>Output:</strong>
2</pre>
<pre>1</pre>
<pre><strong>Explanation of sample case:<br></strong>1)<strong> </strong>In the range [1,5] the K-numbers are 2 and 4 because<br>Divisors of 2 are 1 and 2 which sum up to 3, which is a prime.<br>Divisors of 4 are 1,2 and 4 which sum up to 7, which is a prime.<br>&nbsp;</pre>
<pre>2)<strong> </strong>The K-number in the range [9,10] is 9.</pre>