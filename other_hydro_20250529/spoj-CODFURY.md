<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Infuriated by the Decepticons' defeat after a long epic battle with the Autobots, Megatron, in his rage, has decided to destroy all the planets on his way back to Cybertron from Earth. There are multiple planets between Earth and Cybertron, and each planet has some number of Autobots to guard it from him. Since Megatron is low on ammo, he wants to fight as few autobots as possible (in fact, not more than "M" of them ) on his way back.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You need to find the maximum number of planets he can possibly destroy in his journey.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">NOTE: Megatron can start his "destruction spree" from any planet, and can only move to the next planet from the planet he's currently on.</div>
<p>Infuriated by the Decepticons' defeat after a long epic battle with the Autobots, Megatron, in his rage, has decided to destroy all the planets on his way back to Cybertron from Earth. There are multiple planets between Earth and Cybertron, and each planet has some number of Autobots to guard it from him. Since Megatron is low on ammo, he wants to fight as few autobots as possible on his way back.He can defeat no more than "M" autobots in total.</p>
<p>You need to find the maximum number of planets he can possibly destroy in his journey.</p>
<p>&nbsp;</p>
<p>NOTE: Megatron can start his "destruction spree" from any planet, and can only move to the next planet from the planet he's currently on.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>You will receive one integer "T" denoting the number of test cases. (T&lt;=20)</p>
<p>Then, the next line will contain two non-negative space-separated integers "P" and "M", where P is the number of planets on his way back (P&lt;=50000) and M is the maximum number of Autobots that Megatron can see (M&lt;=1000,000).</p>
<p>After that, one line containing P integers separated by a single space will denote the number of Autobots present in each planet. (For each planet there will be no more than 1000 autobots).</p>
<h3>Output</h3>
<p>Your output should consist of "T" pairs of space-separated integers, one pair per line, denoting the number of Autobots Megatron will fight and the number of planets he will destroy respectively.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
4 50
20 5 23 45

<strong>Output:</strong>
48 3</pre>
<pre>EXPLANATION :&nbsp;</pre>
<pre>Megatron starts at planet 1 (with 20 Autobots) and goes to planet 2, then the 3rd planet,&nbsp;</pre>
<pre>at this point, he has seen 48 Autobots, if he decides to go to planet 4 he will see 93 Autobots��</pre>
<pre>so he stops his journey at the 3rd planet.

Megatron, however, could have started at planet 2 with 5 Autobots, then continue up to the 4th planet, then,&nbsp;</pre>
<pre>he would have seen 73 Autobots, but, as he wants to see the minimum Autobots possible and&nbsp;</pre>
<pre>this number of Autobots exceeds what he wants to see, he decides to choose the way from the 1st to the 3rd planet.</pre>