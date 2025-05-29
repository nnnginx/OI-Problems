<p><img src="/content/ahven:fisher.jpg" alt="A Fishmonger" style="float: right" vspace="3" hspace="8" width="160">A fishmonger wants to bring his goods from the port to the market. On his route he has to traverse an area with many tiny city states. Of course he has to pay a toll at each border.</p>
<p>Because he is a good business man, he wants to choose the route in such a way that he has to pay as little money for tolls as possible. On the other hand, he has to be at the market within a certain time, otherwise his fish start to smell.</p>

<h3>Input</h3>
<p>The first line contains the number of states <i>n</i> and available time <i>t</i>. The first state is the port, the last state is the market. After this line there are <i>n</i> lines with <i>n</i> numbers each, specifying for each state the travel time to the <i>i</i>-th state. This table is terminated with an empty line. The table of the tolls follows in the same format.</p>
<p><i>n</i> is at least 3 and at most 50. The time available is less than 1000. All numbers are integers.</p>
<p>There are many test cases separated by an empty line. Input terminates with number of states and time equal 0 0.</p>
<h3>Output</h3>
<p>For each test case your program should print on one line the total amount of tolls followed by the actual travelling time.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
4 7
0 5 2 3
5 0 2 3
3 1 0 2
3 3 2 0

0 2 2 7
2 0 1 2
2 2 0 5
7 2 5 0

0 0

<b><tt>Sample output:</tt></b>
6 6
</pre>
<p>This corresponds to the following situation, the connections are labeled with (time, toll):</p>
<p><img src="/content/ahven:graf.gif"></p>