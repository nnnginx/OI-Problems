<p>There are exactly N&nbsp;towns in Byteotia. Some towns are connected by bidirectional roads. There are no crossroads outside towns, though there may be bridges, tunnels and flyovers. Each pair of towns may be connected by at most one direct road. One can get from any town to any other-directly or indirectly.</p>
<p>Each town has exactly one citizen. For that reason the citizens suffer from loneliness. It turns out that each citizen would like to pay a visit to every other citizen (in his host's hometown), and do it exactly once. So exactly N*(N-1)&nbsp;visits should take place. That's right,&nbsp;<em>should</em>. Unfortunately, a general strike of programmers, who demand an emergency purchase of software, is under way. As an act of protest, the programmers plan to block one town of Byteotia, preventing entering it, leaving it, and even passing through. As we speak, they are debating which town to choose so that the consequences are most severe.</p>
<h2>Task</h2>
<p>Write a programme that:</p>
<ul>
<li>reads the Byteotian road system's description from the standard input,</li>
<li>for each town determines, how many visits could take place if this town were not blocked by programmers,</li>
<li>writes out the outcome to the standard output.</li>
</ul>
<p>&nbsp;</p>
<h2>Input</h2>
<p>In the first line of the standard input there are two positive integers: N&nbsp;and N&nbsp;(1 &lt;= N &lt;= 100000, 1 &lt;= M &lt;= 500000) denoting the number of towns and roads, respectively. The towns are numbered from 1 to N. The following M&nbsp;lines contain descriptions of the roads. Each line contains two integers X<sub>i</sub>&nbsp;and Y<sub>i</sub>&nbsp;(1 &lt;= X<sub>i</sub>, Y<sub>i</sub> &lt;= N) and denotes a direct road between towns numbered X<sub>i</sub>&nbsp;and Y<sub>i</sub>.</p>
<h2>Output</h2>
<p>Your programme should write out exactly N&nbsp;integers to the standard output, one number per line. The i-th&nbsp;line should contain the number of visits that could not take place if the programmers blocked the town no. i.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>5 5
1 2
2 3
1 3
3 4
4 5</pre>
<p>the correct result is:</p>
<pre>8
8
16
14
8</pre>