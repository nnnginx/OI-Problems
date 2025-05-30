<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Facebook Headquarters - a mysterious, intimidating place, full of magical code and trade secrets. If outsiders were ever to breach the walls of the compound, which are protected by a legion of security guards and, more importantly, security foxes, the entire company could well be brought to its knees!</p>
<p>Actually, wait, tours of the place are given regularly...</p>
<p>The compound consists of $N$ ($1 \leq N \leq 10^5$) buildings, with $M$ ($1 \leq M \leq 10^6$) walkways running amongst them. The $i$th walkway connects buildings $A_i$ and $B_i$ ($1 \leq A_i,B_i \leq N$, $A_i \neq B_i$), and no two buildings are directly connected by more than one walkway. There are no other ways to move from building to building.</p>
<p>Over a period of $D$ ($1 \leq D \leq 10^6$) days, some events will occur at the Headquarters daily. One of two types of events will happen on the $i$th day, indicated by the value of the character $E_i$. If $E_i=$ "T" then a tour will take place - otherwise, $E_i=$ "S", and a security sweep of a building will take place.</p>
<p>If a tour is given on the $i$th day, visitors will enter the compound at building $X_i$, and leave from building $Y_i$ ($1 \leq X_i,Y_i \leq N$, $X_i \neq Y_i$). If it turns out that these two buildings are not actually connected by any sequence of walkways, then the tour will be cancelled, and the unfortunate visitors will be given Facebook T-shirts and promptly kicked out. Otherwise, a large number of groups of people will be led from building $X_i$ to building $Y_i$ along various routes. No route will involve travelling along the same walkway multiple times (even in different directions), but a route might revisit the same building repeatedly, including buildings $X_i$ and $Y_i$. Along the way, some visitors will inevitably get "lost", and fail to rejoin their tour group. How many of them will get away with this will depend on the security levels that day, but it's safe to say that, in total, $O_i$ ($1 \leq O_i \leq 1000$) new outsiders will be left behind in each building which could possibly be part of any valid tour route from building $X_i$ to building $Y_i$. Good thing they'll no doubt have brought cameras to amuse themselves with while they wait to be found.</p>
<p>On the other hand, if a security sweep is conducted on the $i$th day, then the security guards (and foxes) will carefully search building $Z_i$ ($1 \leq Z_i \leq N$) for any trespassers remaining from previous tours, who will be kindly escorted out of the Headquarters (after being given Facebook T-shirts for the road, of course).</p>
<p>Because this company likes to collect data about everything, you've been hired to record how many outsiders were found in each sweep. However, to make things more interesting, you'll instead simply write a program to predict these values based on the map of the compound and the schedule of events!</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $T$ ($1 \leq T \leq 20$), the number of test cases</p>
<p><strong>For each test case:</strong></p>
<p>Line 1: 3 integers, $N$, $M$, and $D$</p>
<p>Next $M$ lines: 2 integers, $A_i$ and $B_i$, for $i=1..M$</p>
<p>Next $D$ lines: 1 character, $E_i$, followed by the three integers $X_i$, $Y_i$, and $O_i$ if $E_i=$ "T", or the single integer $Z_i$ if $E_i=$ "S", for $i=1..K$</p>
<h3>Output</h3>
<p><strong>For each test case:</strong></p>
<p>1 integer, the total number of people escorted out of the compound, modulo $10^9+7$</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>6 5 9<br>1 2<br>2 3<br>3 4<br>4 5<br>5 3<br>T 1 2 5<br>T 5 6 1000<br>S 2<br>S 6<br>T 2 3 1<br>T 5 3 14<br>S 1<br>S 2<br>S 4</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">26</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>On the first day, a tour is given from building 1 to building 2. The only valid route consists of simply crossing the walkway between these two buildings. As such, by the end of the day, 5 outsiders are left hiding in each of buildings 1 and 2.</p>
<p>On the second day, the planned low-security tour unfortunately cannot take place, due to no routes existing between buildings 5 and 6. Facebook should probably hire some new tour planners, as well as architects.</p>
<p>On the following two days, security sweeps of buildings 2 and 6 are carried out, with 5 and 0 outsiders found and removed, respectively.</p>
<p>On the fifth day, a tour is given from building 2 to building 3. There are exactly three valid routes, passing through buildings 2-3, 2-3-4-5-3, and 2-3-5-4-3. As such, one new outsider remains behind in each of buildings 2, 3, 4, and 5.</p>
<p>On the sixth day, a tour is given from building 5 to building 3. There are exactly two valid routes, passing through buildings 5-3 and 5-4-3. As such, 14 new outsiders take up residence in each of buildings 3, 4, and 5.</p>
<p>Finally, security sweeps of buildings 1, 2, and 4 are conducted, evicting 5, 1, and 15 people, respectively. In total, then, 5+0+5+1+15=26 people will have been escorted out of the compound, which is still 26 when taken modulo $10^9+7$. Following these events, buildings 3 and 5 still contain 15 outsiders, while the others contain none.</p>