<p>Factorial is one of the most attractive word this week, it is proposed to reload a famous <a href="http://www.spoj.com/problems/DCEPC11B/">problem</a>. Is it so boring ? 
<br>
As the <a href="http://www.spoj.com/problems/BORING/">reload edition</a> wasn't hard enough, we'll extend constraints.
<br>
<br>
<br>

Sameer and Arpit want to overcome their fear of Maths and so they have been recently practicing Maths problems a lot. Aman, their friend has been helping them out. But as it goes, Sameer and Arpit have got bored of problems involving factorials. Reason being, the factorials are too easy to calculate in problems as they only require the residue modulo some prime and that is easy to calculate in linear time. So to make things interesting for them, Aman - The Mathemagician, gives them an interesting task. He gives them a prime number <strong><em>P</em></strong> and an integer <strong><em>N</em></strong> (not so) close to <strong><em>P</em></strong>, and asks them to find <strong><em>N! modulo P</em></strong>. He asks <strong><em>T</em></strong> such queries.
</p>


<h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
two integers <strong><em>N</em></strong>, and <strong><em>P</em></strong> a prime number.
</p>

<h3>Output</h3>
<p>For each test case, you have to print <strong><em>N! modulo P</em></strong>.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
2 5
5 11
21 71
</pre>
<pre><strong>Output:</strong>
2
10
6
</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^3
0 &lt; N &lt; 10^100
1 &lt; P &lt; 10^100, a prime number
Abs(N-P) &lt; 10^6
</pre>
<p></p>

<p>Problem designed to be solvable using some 'slow' languages like Python (333B of code) in the third of the time_limit.<br>

<b>Warning</b> : To get AC here, you need to get around 1000 points (approx) in <a href="http://www.spoj.com/problems/BORING3/">challenge edition</a>.<br>
My best python code get AC under 5s. (edit 2017-02-11, after compiler changes)<br>

;-) Have fun.</p>