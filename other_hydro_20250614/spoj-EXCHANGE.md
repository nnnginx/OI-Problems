<p>There are 3 kinds of money in a planet far away from the earth: Mone, Luck, and Rpin. There's a money exchange company in this planet. You must go to this company if you want to do some money exchange, and, more autocratically, this company regulate the exchange rate of each pair of these 3 kinds of money. </p>
<p>The money exchange will be done in the following two ways:</p>
<p>(A)</p>
<p>You give the company a real number <i>x</i> in the range (0,100], the company will exchange <i>x</i>% of your Mone and <i>x</i>% of your Luck to equal Rpin according to the exchange rate of that day.</p>
<p>(B)</p>
<p>You give the company a real number <i>x</i>, the company will exchange your <i>x</i> Rpin to some Mone and Luck, whose value is equal to <i>x</i> Rpin according to the exchange rate of that day, and, the value of Mone is <i>Rate</i> times of the value of Luck.</p>
<p>You can do many exchange operations in the same day.</p>
<p>Now, as the excellant spy in this planet, you know the exchange rate between Mone and Rpin of each of the next <i>n</i> days(a<sub>i</sub> Mone per Rpin), and the exchange rate between Luck and Rpin of each of the next <i>n</i> days(b<sub>i</sub> Luck per Rpin), and, each Rate of the next <i>n</i> days( Rate<sub>i</sub>). you have <i>S</i> Rpin in the start, and you want to get most Rpin in the <i>n</i>th day later.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them( &lt;=5 ) is given in the very first line.</p>
<p>For each test case: </p>
<p>The first line contains a integer number n(1&lt;=n&lt;=100000) and a real number S.n lines follow, each contains 3 real numbers: a<sub>i</sub>(between 0 and 10), b<sub>i</sub>(between 0 and 10), Rate<sub>i</sub>(between 0 and 100).</p>
<h3>Output</h3>
<p>For each test case, output one line contains a real number with 3 digits after decimal point, which denotes to the answer. You can assume it is less than 1000000000.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
3 100
1 1 1
1 2 2
2 2 3

<b>Output:</b>
225.000
</pre>
<b>Warning: large input/output data, be careful with certain languages; the time limit is somewhat strict for this problem</b>