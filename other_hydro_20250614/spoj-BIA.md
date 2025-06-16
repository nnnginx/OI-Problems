<p>Bytelandian Information Agency (BIA) uses a net of <i>n</i> computers.
The computers are numbered from <i>1</i> to <i>n</i>, and
the computer number <i>1</i> is a server. The computers are connected
by one-way information channels. Every channel connects a pair of computers.
The whole network is organised in such a way that one can send information
from the server to any other computer either directly or indirectly.
</p>
<p>
When BIA acquires new information, the information is put on the server
and propagated in the net. The chief of BIA considers what would happen
if one computer stopped working (was blown away by terrorists for example).
It could happen that some other computers would stop receiving information
from the server, because the broken computer was a necessary transmitter.
We will call such computers <i>critical</i>. For example in the situation
in the picture below the critical computers are <i>1</i> and <i>2</i>. <i>1</i>
is the server and all information sent from the server to <i>3</i> has to go
through <i>2</i>.
</p>
<img src="/content/kfas:BIA.gif" alt="BIA computer net" width="300" height="249" border="0/">
<h3> Task </h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li> reads a description of the net from standard input,
</li>
<li> finds all critical computers.
</li>
<li> writes the numbers of critical computers to standard output.
</li>
</ul></div>
<h3> Input </h3>
<p>
Ten test cases (given one under another, you have to process all!).
Each test case consists of several lines.
In the first line there are numbers <i>n</i> and <i>m</i>. <i>n</i> denotes
the number of computers in the net,<i>(2&lt;=n&lt;=5000)</i>. <i>m </i> denotes the
number of information
channels, <i>n-1&lt;=m&lt;=200000</i>. The following <i>m</i> lines describes a single information
channel and consist of two integer numbers <i>a</i> and <i>b</i> separated by a space.
It means the computer <i>a</i> sends information to computer <i>b</i> by that channel.
You may assume there are no two channels which start and end at the same points <i>a, b</i>.
</p>
<h3> Output </h3>
<p>
For every testcase your program should write two lines. In the first line
<i>k</i> - the number of critical computers in the net. In the second line
<i>k</i> numbers separated by single spaces - the numbers of critical computers in increasing order.
</p>
<h3>Example</h3>
<pre><tt><b>Input:</b>
4 5
1 2
1 4
2 3
3 4
4 2
[and 9 test cases more]
</tt>
<tt><b>Output:</b>
2
1 2
[and 9 test cases more]
</tt>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>