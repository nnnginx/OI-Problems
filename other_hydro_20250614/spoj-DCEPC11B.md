<p>Sameer and Arpit want to overcome their fear of Maths and so they have been recently practicing Maths problems a lot. Aman, their friend has been helping them out. But as it goes, Sameer and Arpit have got bored of problems involving factorials. Reason being, the factorials are too easy to calculate in problems as they only require the residue modulo some prime and that is easy to calculate in linear time. So to make things interesting for them, Aman - The Mathemagician, gives them an interesting task. He gives them a prime number P and an integer N close to P, and asks them to find N! modulo P. He asks T such queries.</p>
<h3>Input</h3>
<p>First line contains an integer T, the number of queries asked.</p>
<p>Next T lines contains T queries of the form ¡°N P¡±. (quotes for clarity)</p>
<h3>Output</h3>
<p>Output exactly T lines, containing N! modulo P.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
2 5
5 11
21 71

<strong>Output:</strong>
2
10
6</pre>

<strong>Constraints:</strong><p></p><p>1 &lt;= T &lt;= 1000</p><p>1 &lt; P &lt;= 2*10^9</p><p>1 &lt;= N &lt;= 2*10^9</p>
Abs(N-P) &lt;= 1000