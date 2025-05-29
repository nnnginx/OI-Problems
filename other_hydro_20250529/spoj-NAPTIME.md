<p>Goneril is a very sleep-deprived cow. Her day is partitioned into
N (3 &lt;= N &lt;= 3,830) equal time periods but she can spend only B (2
&lt;= B &lt; N) not necessarily contiguous periods in bed.  Due to her
bovine hormone levels, each period has its own utility U_i (0 &lt;=
U_i &lt;= 200,000), which is the amount of rest derived from sleeping
during that period.  These utility values are fixed and are independent
of what Goneril chooses to do, including when she decides to be in
bed.<br><br>

With the help of her alarm clock, she can choose exactly which
periods to spend in bed and which periods to spend doing more
critical items such as writing papers or watching baseball. However,
she can only get in or out of bed on the boundaries of a period.<br><br>

She wants to choose her sleeping periods to maximize the sum of the
utilities over the periods during which she is in bed.  Unfortunately,
every time she climbs in bed, she has to spend the first period
falling asleep and gets no sleep utility from that period.<br><br>

The periods wrap around in a circle; if Goneril spends both periods
N and 1 in bed, then she does get sleep utility out of period 1.<br><br>

What is the maximum total sleep utility Goneril can achieve?<br>
</p>

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases, then <i>t</i> test cases follow. <br>
Each test case takes the following form:<br>
Two space-separated integers: <i>N</i> and <i>B</i>, then <i>N</i> lines follows<br>
Each line contains a single integer, <i>U_i</i>, between 0 and 200,000 inclusive <br>

</p><h3>Output</h3>
<p>For each test case output a single integer, the maximum total sleep utility Goneril can achieve. <br>

</p><h3>Example</h3>
<pre><b>Input:</b>
1
5 3
2
0
3
1
4

<b>Output:</b>
6

<b>Input/Output details:</b>
The day is divided into 5 periods, with utilities 2, 0, 3, 1, 4 in that 
order. Goneril must pick 3 periods.

Goneril can get total utility 6 by being in bed during periods 4,
5, and 1, with utilities 0 [getting to sleep], 4, and 2
respectively.
</pre>