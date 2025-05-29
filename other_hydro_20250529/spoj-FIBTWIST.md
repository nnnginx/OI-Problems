<p>Fibonacci numbers are given by&nbsp;</p>
<ul>
  <li>f(n) = f(n-1) + f(n-2)</li>
</ul>
<p>with f(0) = 0 &amp; f(1) = 1.</p>
<p>first number of series ------ 0 &nbsp;1 &nbsp;1 &nbsp;2 &nbsp;3 &nbsp;5 &nbsp;8 &nbsp;13&nbsp;</p>

<p>Now let's have a new series called "Fibonacci Twist" which is given by&nbsp;</p>
<ul>
  <li>ft(n) = ft(n-1) + ft(n-2) + (n-1) </li>
</ul>
<p>with ft(0) = 0 &amp; ft(1) = 1.</p>
<p>with first few number in the series ----- 0 &nbsp;1 &nbsp;2 &nbsp;5 &nbsp;10 &nbsp;19 &nbsp;34 &nbsp;59&nbsp;</p>

<p>&nbsp;</p>
<p>Now your task is to find ft(n).</p>
<p>Since the number can be Big you have to find the result mod M.</p>

<h3>Input</h3>
<p>first line having single number 't' -- number of test cases.</p>
<p>next t lines have 2 number each 'n' and 'M'</p>

<h3>Output</h3>
<p>Single number given the n-th term mod M</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 20
10 77
15 111

<strong>Output:</strong>
19
45
69</pre>

<h3>Constraints</h3>
<ul>
  <li>10 &lt;= t &lt;= 100</li>
  <li>0 &lt;= n &lt;= 10^9</li>
  <li>100 &lt;= M &lt;= 10^9</li>
</ul>

<h3>Explanation</h3>
<ol>
  <li>ft(5) is 19. 19 % 20 = 19</li>
  <li>ft(10) is 276.  276 % 77  = 45</li>
  <li>ft(15) is 3177. 3177 % 111 = 69</li>
</ol>