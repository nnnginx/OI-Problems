<p>FJ has purchased N (1 &lt;= N &lt;= 2000) yummy treats for the cows who
get money for giving vast amounts of milk. FJ sells one treat per
day and wants to maximize the money he receives over a given period
time.
The treats are interesting for many reasons:
  </p>
<ul>
	<li> The treats are numbered 1..N and stored sequentially in single
    file in a long box that is open at both ends. On any day, FJ
    can retrieve one treat from either end of his stash of treats.
  </li>
	<li>Like fine wines and delicious cheeses, the treats improve with
    age and command greater prices.</li>
	<li>The treats are not uniform: some are better and have higher
    intrinsic value. Treat i has value v(i) (1 &lt;= v(i) &lt;= 1000).
  </li>
	<li>Cows pay more for treats that have aged longer: a cow will
    pay v(i)*a for a treat of age a.

	</li>
</ul>
<p>Given the values v(i) of each of the treats lined up in order of
the index i in their box, what is the greatest value FJ can receive
for them if he orders their sale optimally?

</p>
<p>The first treat is sold on day 1 and has age a=1. Each subsequent
day increases the age by 1.</p>
<h3>Input</h3>
<p>Line 1: A single integer, N</p>
<p>Lines 2..N+1: Line i+1 contains the value of treat v(i)</p>

<h3>Output</h3>
<p>The maximum revenue FJ can achieve by selling the treats</p><h3>Example</h3>

<pre><b>Input:</b>
5
1
3
1
5
2

<b>Output:</b>
43</pre>