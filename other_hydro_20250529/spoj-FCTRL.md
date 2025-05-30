<p>
The most important part of a&nbsp;GSM network is so called
<em>Base Transceiver Station</em> (<em>BTS</em>). These transceivers form the
areas called <em>cells</em> (this term gave the name to the cellular phone)
and every phone connects to the BTS with the strongest signal (in
a&nbsp;little simplified view). Of course, BTSes need some attention and
technicians need to check their function periodically.

</p><p>
ACM technicians faced a&nbsp;very interesting problem recently. Given a&nbsp;set of
BTSes to visit, they needed to find the shortest path to visit all of the
given points and return back to the central company building. Programmers
have spent several months studying this problem but with no results. They
were unable to find the solution fast enough. After a&nbsp;long time, one of the
programmers found this problem in a&nbsp;conference article. Unfortunately, he
found that the problem is so called "Travelling Salesman Problem" and it is
very hard to solve. If we have <var>N</var> BTSes to be visited, we can visit them in
any order, giving us <var>N</var>! possibilities to examine. The function expressing
that number is called factorial and can be computed as a&nbsp;product

1.2.3.4....<var>N</var>. The number is very high even for a&nbsp;relatively small <var>N</var>.

</p><p>
The programmers understood they had no chance to solve the problem. But
because they have already received the research grant from the government,
they needed to continue with their studies and produce at least <em>some</em>
results. So they started to study behaviour of the factorial function.

</p><p>
For example, they defined the function <var>Z</var>. For any positive integer <var>N</var>,
<var>Z</var>(<var>N</var>) is the number of zeros at the end of the decimal form of number
<var>N</var>!. They noticed that this function never decreases. If we have two numbers
<var>N</var><sub>1</sub>&lt;<var>N</var><sub>2</sub>, then 
<var>Z</var>(<var>N</var><sub>1</sub>) &lt;= <var>Z</var>(<var>N</var><sub>2</sub>). It is because we can never "lose" any
trailing zero by multiplying by any positive number. We can only get new
and new zeros. The function <var>Z</var> is very interesting, so we need a&nbsp;computer
program that can determine its value efficiently.

</p><p>
</p><h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 100000). It stands
for the number of numbers to follow. Then there are <var>T</var> lines, each containing
exactly one positive integer number <var>N</var>, 
1 &lt;= <var>N</var> &lt;= 1000000000.

</p><p>
</p><h3>Output</h3>

<p>
For every number <var>N</var>, output a&nbsp;single line containing the single non-negative
integer <var>Z</var>(<var>N</var>).
</p><h3>Example</h3>
<p>Sample Input:</p>

<pre><tt>6
3
60
100
1024
23456
8735373
</tt></pre>

<p>Sample Output:</p>

<pre><tt>0
14
24
253
5861
2183837
</tt></pre>