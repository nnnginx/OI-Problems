<p>The interconnection of the relays in a cable TV network is bi-directional. The network is connected if there is at least one interconnection path between each pair of relays present in the network. Otherwise the network is disconnected. An empty network or a network with a single relay is considered connected. The safety factor <b>f</b> of a network with <b>n</b> relays is:</p>
<p>1. <b>n</b>, if the net remains connected regardless the number of relays removed from the net.
<br>2. The minimal number of relays that disconnect the network when removed.</p>
<img src="/content/thanhvy:cabletv.jpg" alt="Exemplary illustration">

<p>For example, consider the nets from figure 1, where the circles mark the relays and the solid lines correspond to interconnection cables. The network (a) is connected regardless the number of relays that are removed and, according to rule (1), f=n=3. The network (b) is disconnected when 0 relays are removed, hence f=0 by rule (2). The network (c) is disconnected when the relays 1 and 2 or 1 and 3 are removed. The safety factor is 2.</p>

<h3>Input</h3>
<p>The input starts with a line containing a single integer <b>t</b> &lt;= 20, the number of test cases. <b>t</b> test cases follow.</p>
<p>Write a program that computes the safety factor for the cable networks encoded by the data sets. Each data set starts with two integers: 0 &lt;= <b>n</b> &lt;=50,the number of relays in the net, and <b>m</b>, the number of cables in the net. Follow <b>m</b> data pairs (u,v), u &lt; v, where u and v are relay identifiers (integers in the range 0..<b>n</b>-1). The pair (u,v) designates the cable that interconnects the relays u and v. The pairs may occur in any order. Except the (u,v) pairs, which do not contain white spaces, white spaces can occur freely in input. Input data terminate with an end of file and are correct.</p>

<h3>Output</h3>
<p>For each data set, prints from the beginning of a line, the safety factor of the encoded net.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5
0 0
1 0
3 3 (0,1) (0,2) (1,2)
2 0
5 7 (0,1) (0,2) (1,3) (1,2) (1,4) (2,3) (3,4)

<b>Output:</b>
0
1
3
0
2
</pre>