<p>
In order to celebrate the 2nd anniversary of Travel Agent SPOJ (Safe 每 Professional 每 hOspitable 每 Joyful), the management intend to hold free tours around cities for clients to make them more satisfied with SPOJ. 
</p>
<p>
A tour is a simple cycle, starting at any city (called a source-city) visits some other cities (each city must be visited at most once) and then returns to the source-city. The number of roads in the tour should be an even number because we are celebrating a 2nd anniversary, and 2 is even! Since many tours in different areas of the country are planned, the cost of organising them could turn out quite high. Hence, the management of SPOJ hope to find at least one 'reasonable' tour, which should have as small a number of roads as possible. 
</p>

<p> 
You're given maps of the areas where SPOJ wants to hold free tours. For each map, help them figure out a reasonable tour.
</p>

<h3>Input</h3>
<p>
The first line of input contains an integer <b>t</b>, the number of maps (<b>t</b> &lt;= 5). <b>t</b> maps follow. 
</p>

<p>
For each map:
</p>
<ul>
<li> In the first line there are 2 integers <b>N</b> 每 number of cities in that area, <b>M</b> 每 number of roads (1 &lt;= <b>N</b> &lt;= 8000, 0 &lt;= <b>M</b> &lt;= 10000)</li>
<li> In the next <b>M</b> lines, the i-th line describes the i-th road: a line with two integers <b>a b</b> denotes a bidirectional road between city <b>a</b> and city <b>b</b> </li>
</ul>
<p>There is one blank line between successive tests.</p>

<h3>Output</h3>
<p>For each map, if there is no tour satisfying the conditions, write "-1" (without quotes). Otherwise, write one integer representing the number of roads in a reasonable tour, and in the next line show out the tour with form "source-city a b c .. source-city", that means the tour is source-city -&gt; city a -&gt; city b -&gt; ＃ -&gt; source-city. If there are many tours satisfy in each map, any of them will be accepted.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2

3 3
1 2 
2 3
3 1

4 4
1 2
2 3
3 4
4 1


<b>Output:</b>
-1
4
1 2 3 4 1
</pre>