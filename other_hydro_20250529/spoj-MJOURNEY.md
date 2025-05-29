<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MJOURNEY/en/">English</a></td>
<td width="50%"><a href="/problems/MJOURNEY/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<pre>Farmer John has a pig farm near town A. He wants to visit his friend living
in town B. During this journey he will visit n small villages so he decided
to earn some money. He tooks n pigs and plans to sell one pig in each 
village he visits. Pork prices in villages are diﬀerent, in the j-th village
the people would buy a pork at pj rubles per kilogram. The distance from town
A to the j-th village along the road to town B is dj kilometers.
Pigs have diﬀerent weights. Transporting one kilogram of pork per one kilometer
of the road needs t rubles for addition fuel.

Help John decide, which pig to sell in each town in order to earn as much money
as possible.
</pre>
<h3>Input</h3>
<pre>The ﬁrst line of the input ﬁle contains integer numbers n (1 ≤ n ≤ 1000) and t
(1 ≤ t ≤ 10^9). The second line contains n integer numbers wi (1 ≤ wi ≤ 10^9) 
— the weights of the pigs. The third line contains n integer numbers dj 
(1 ≤ dj ≤ 10^9) — the distances to the villages from the town A. The fourth line
contains n integer numbers pj (1 ≤ pj ≤ 10^9) — the prices of pork 
in the villages.

SAMPLE INPUT
3 1
10 20 15
10 20 30
50 70 60
</pre>
<h3>Output</h3>
<pre> 
Output n numbers, the j-th number is the number of pig to sell in the j-th village. 
The pigs are numbered from 1 in the order they are listed in the input ﬁle.

SAMPLE OUTPUT
3 2 1
</pre>
<p> </p>