<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/OTOCI/en/">English</a></td> 
<td width="50%"><a href="/problems/OTOCI/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Some time ago Mirko founded a new tourist agency named "Dreams of Ice". The agency purchased N
icy islands near the South Pole and now offers excursions. Especially popular are the emperor
penguins, which can be found in large numbers on the islands.</p>
<p>Mirko's agency has become a huge hit; so big that it is no longer cost-effective to use boats for the
excursions. The agency will build bridges between islands and transport tourists by buses. Mirko
wants to introduce a computer program to manage the bridge building process so that fewer mistakes
are made.</p>
<p>The islands are numbered 1 through N. No two islands are initially connected by bridges. The initial
number of penguins on each island is known. That number may change, but will always be between 0
and 1000 (inclusive).</p>
<p>Your program must handle the following three types of commands:
</p><ul>
<li>"bridge A B" �C an offer was received to build a bridge between islands A and B (A and B will
be different). To limit costs, your program must accept the offer only if there isn't already a
way to get from one island to the other using previously built bridges. If the offer is accepted,
the program should output "yes", after which the bridge is built. If the offer is rejected, the
program should output "no".</li>
<li>"penguins A X" �C the penguins on island A have been recounted and there are now X of them.
This is an informative command and your program does not need to respond.</li>
<li>"excursion A B" �C a group of tourists wants an excursion from island A to island B. If the
excursion is possible (it is possible to get from island A to B), the program should output the
total number of penguins the tourists would see on the excursion (including islands A and B).
Otherwise, your program should output "impossible".</li>
</ul>
<p></p>

<h3>Input</h3>
<p>The first line contains the integer N (1 �� N �� 30 000), the number of islands.</p>
<p>The second line contains N integers between 0 and 1000, the initial number of penguins on each of the
islands.</p>
<p>The third line contains an integer Q (1 �� Q �� 300 000), the number of commands.</p>
<p>Q commands follow, each on its own line.</p>

<h3>Output</h3>
<p>Output the responses to commands "bridge" and "excursion", each on its own line.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5
4 2 4 5 6
10
excursion 1 1
excursion 1 2
bridge 1 2
excursion 1 2
bridge 3 4
bridge 3 5
excursion 4 5
bridge 1 3
excursion 2 4
excursion 2 5

<b>Output:</b>
4
impossible
yes
6
yes
yes
15
yes
15
16


<b>Input:</b>
6
1 2 3 4 5 6
10
bridge 1 2
bridge 2 3
bridge 4 5
excursion 1 3
excursion 1 5
bridge 3 4
excursion 1 5
penguins 3 10
excursion 1 3
bridge 1 5

<b>Output:</b>
yes
yes
yes
6
impossible
yes
15
13
no
</pre>