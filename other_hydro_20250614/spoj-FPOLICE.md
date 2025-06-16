<p>Dhamaka Singh (a crook) has just robbed a bank and would like to get out of the country as soon as possible. But there is a slight problem, the police!  On his way out of the country he has to pass through some police stations. Each police station has a certain risk (for Dhamaka Singh) associated with it.  He wants to get to the airport within a certain time <b>T</b> or else he'll miss his flight.  He also wants to take a path that minimizes the total risk associated with it.  Help Dhamaka Singh get out of the country.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>The first line of each test case contains 2 integers <b>N</b> (3 &lt;= <b>N</b> &lt;= 100) and <b>T</b> (1 &lt;= <b>T</b> &lt;= 250), denoting the number of police stations and the total time he has to reach the airport, respectively.</p>

<p>Dhamaka Singh has to start from the first police station and reach the <b>N</b><sup>th</sup> one (the airport is just after the <b>N</b><sup>th</sup> police station).  You can consider the time taken between the <b>N</b><sup>th</sup> police station and the airport to be negligible.</p>

<p>Next there are <b>N</b> lines with <b>N</b> numbers in each line, separated by single spaces.  All numbers are separated by a single space. The j<sup>th</sup> integer in the i<sup>th</sup> line represents the time taken to reach the j<sup>th</sup> police station from the i<sup>th</sup> police station.

</p><p>Next there are another <b>N</b> lines with <b>N</b> numbers in each line.  All numbers are separated by a single space.  The j<sup>th</sup> integer in the i<sup>th</sup> line represents the risk involved in travelling to the j<sup>th</sup> police station from the i<sup>th</sup> police station.</p>

<h3>Output</h3>
<p>For each test case output one line containing 2 integers separated by a single space.</p>

<p>The first integer denotes the minimum total risk to reach the airport.  The second integer denotes the minimum time required to reach the airport at the minimum total risk.</p>

<p>If it is impossible to reach the airport within time <b>T</b> (inclusive), just print "-1" (quotes for clarity).</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
4 10
0 6 2 3
6 0 2 3
3 1 0 2
3 3 2 0
0 2 2 7
2 0 1 2
2 2 0 5
7 2 5 0

<b>Output:</b>
4 9
</pre>