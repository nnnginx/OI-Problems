<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>It's down to the final match in the world's biggest SC2$^1$ tournament! You're the MVP$^2$ of MVP$^3$, and you're going up against MVP$^4$. There are $G$ ($1 \leq G \leq 20$) games in the series, with a winner decided after all have been played. Being a Protoss$^5$ player, you know the perfect way to win against that Terran$^6$ scum - with a cannon rush$^7$ every single game. Now you just have to execute it perfectly, by quickly getting your probe$^{10}$ to the correct location, and the prize money's sure to be yours.</p>
<p>Each game will take place on a map which can be represented as a grid with $H$ ($2 \leq H \leq 1000$) rows of $W$ ($2 \leq W \leq 1000$) cells each. Each cell contains either empty space (represented by "E"), water ("W"), a unit ("U"), one of exactly two mineral patches ("M"), the probe ("P"), or the cannon rush site ("C"). Every second, your probe can move to a horizontally- or vertically-adjacent cell within the grid, with the goal of reaching the cannon rush site in as little time as possible. It can move freely from an empty cell to another empty cell (including its initial position and destination), while cells containing water or minerals may never be traversed.</p>
<p>Normally, the probe may also not pass through units. However, it <em>can</em>&nbsp;if it is travelling towards a mineral patch. Specifically, the probe can only leave or enter a cell containing a unit if, for at least one of the two mineral patches on the map, the cell which the probe is entering is closer to that patch than the cell which the probe is leaving. Closeness is defined according to the minimum amount of time it would take to reach the mineral patch from the given cell, assuming the ability to pass through all units on the way.</p>
<p>For each game, you'd like to determine whether or not you can be successful in your strategy, and, if so, how quickly you can execute the cannon rush. Of course, the point of this is to help prepare the correct BM$^{11}$ for the end of the game.</p>
<h3>Input</h3>
<p>First line: 1 integer, $G$</p>
<p>For each game:</p>
<p>First line: 2 integers, $H$ and $W$</p>
<p>Next $H$ lines: $W$ characters, representing the $i$th row of the map, for $i = 1..H$</p>
<h3>Output</h3>
<p>For each game:</p>
<p>The BM to be typed at the conclusion of the game. Namely, if the probe can reach the cannon rush site, the string "pwned you in $X$ seconds eZ$^{12}$, learn to play n00b$^{13}$" (without the quotes and glossary numbers), where $X$ is the minimum number of seconds for it to do so - otherwise, the string "terran so broken, apologize for playing this race".</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>4 5<br>WWEMC<br>EEEUE<br>PUWWU<br>MEEEE<br>5 4<br>EWEM<br>ECUE<br>EEWE<br>EWEE<br>EUPM</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">pwned you in 8 seconds eZ, learn to play n00b<br>terran so broken, apologize for playing this race</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>In the first scenario, the single shortest path that the probe may take to the cannon rush site is illustrated below:</p>
<p><img src="../../../content/sourspinach:uoftbe.bmp" alt=""></p>
<p>Note that the first move is made by going "towards" the top-right mineral patch, while the second move is made by going towards the bottom-left one.</p>
<p>In the second scenario, the probe is unable to pass through any of the units, due to the locations of the mineral patches, and as such cannot reach its destination.</p>
<pre><strong>Glossary of Terms:</strong></pre>
<p>$^1$ <strong>SC2:</strong> StarCraft 2, by Blizzard Entertainment - a game of kings</p>
<p>$^2$ <strong>MVP:</strong>&nbsp;Most valuable player</p>
<p>$^3$ <strong>MVP:</strong>&nbsp;A top Korean SC2 team</p>
<p>$^4$ <strong>MVP:</strong>&nbsp;A top Korean Terran player (who is not on the team MVP)</p>
<p>$^5$ <strong>Protoss:</strong>&nbsp;The most pleasant race in SC2, which only nice people use</p>
<p>$^6$ <strong>Terran:</strong>&nbsp;The most despicable race in SC2, which no decent human being would consider&nbsp;</p>
<p>$^7$ <strong>Cannon rush:</strong>&nbsp;The act of building proxy$^8$ cannons, a common type of cheese$^9$</p>
<p>$^8$ <strong>Proxy:</strong>&nbsp;A structure made near or in your opponent's base, instead of your own</p>
<p>$^9$ <strong>Cheese:</strong>&nbsp;A perfectly legitimate strategy which can allow you to win quickly, while leaving your opponent mad</p>
<p>$^{10}$ <strong>Probe:</strong>&nbsp;A Protoss unit most useful for its ability to make cannons</p>
<p>$^{11}$ <strong>BM:</strong>&nbsp;Customary parting words for your opponent, used to convey your respect for them</p>
<p>$^{12}$ <strong>eZ:</strong> Easy</p>
<p>$^{13}$ <strong>n00b:</strong>&nbsp;A player whose skill is somewhat lacking in calibre</p>