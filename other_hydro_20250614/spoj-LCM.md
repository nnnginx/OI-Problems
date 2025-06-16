<p>There are no days and nights on byte island, so the residents here can hardly determine the length of a single day. Fortunately, they have invented a clock with several pointers. They have <b>N</b> pointers which can move round the clock. Every pointer ticks per second, and the <i>i</i>-th pointer move to the start position after <i>i</i> times of ticks. The wise of the byte island decide to define a day as the time interval between the start time and the first time when all the pointers moves to the position exactly the same as the start time.
The wise of the island decide to choose some of the <b>N</b> pointers to make the length of the day are greater than or equal to a given seconds <b>M</b>. They want to know how many different ways to make it possible.

</p><h3>Input</h3>

<p>There are a lot of test cases, the number of test cases are in the first line of input.
</p><p>For each test cases, there are only one line contains two integers <b>N</b> and <b>M</b>, indicating the number of pointers and the lower bound for seconds of a day. (1 &lt;= <b>N</b> &lt;= 40, 1 &lt;= <b>M</b> &lt;= 2<sup>63</sup>-1)

</p><h3>Output</h3>

<p>For each test case, output a single integer denoting the number of ways.</p>

<h3>Example</h3>
<pre><b>Input:</b>
3
5 5
10 1
10 128

<b>Output:</b>
Case #1: 22
Case #2: 1023
Case #3: 586
</pre>