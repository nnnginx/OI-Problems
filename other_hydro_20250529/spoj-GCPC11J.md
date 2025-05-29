<p>As you might know, most computer networks are organized in a tree-like fashion, i.e. each computer is reachable by each other computer but only over one, unique path.</p>
<p>The so-called <em>Time to live</em> (TTL) specifies after how many hops a network packet is dropped if it has not reached its destination yet. The purpose of the TTL is to avoid situations in which a packet circulates through the network caused by errors in the routing tables.</p>
<p>The placement of a router that connects the network to another network is optimal when the maximal needed TTL for packets that are sent from this router to any other computer within the same network is minimal. Given a network as specified above, you should calculate the maximal needed TTL in this network if you can select the computer that should be used as router.</p>
<h3>Input</h3>
<p>The first line of the input consists of the number of test cases <em>c</em> that follow (<em>1 ¡Ü c ¡Ü 100</em>). Each test case starts with a line specifying <em>N</em>, the number of computers in this network (<em>1 &lt; N ¡Ü 10<sup>5</sup></em>). Computers are numbered from <em>0</em> to <em>N-1</em>. Then follow <em>N-1</em> lines, each specifying a network connection by two numbers <em>a</em> and <em>b</em> which means that computer <em>a</em> is connected to computer <em>b</em> and vice versa, of course (<em>0 ¡Ü a,b &lt; N</em>).</p>
<h3>Output</h3>
<p>For each test case in the input, print one line containing the optimal TTL as specified above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
2
1 0
5
3 2
2 1
0 2
2 4
9
3 1
6 5
3 4
0 3
8 1
1 7
1 6
2 3

<strong>Output:</strong>
1
1
2
</pre>