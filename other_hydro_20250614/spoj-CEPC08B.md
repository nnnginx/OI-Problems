<p>In a seaside village, there is an avenue of skyscrapers. Each skyscrapers is 100m wide and has certain
height. Due to very high price of parcels, any two consecutive skyscrapers are adjacent. The avenue lies close to the beach so the street is exactly at the sea level.
Unfortunately, this year, due to the global warming, the sea level started to increase by one meter
each day. If the skyscraper height is no greater than the current sea level, it is considered ﬂooded.
A region is a maximal set of non-ﬂooded, adjacent skyscrapers. This term is of particular importance, as
it is suﬃcient to deliver goods (like current, carrots or cabbages) to any single skyscraper in each region.
Hence, the city major wants to know how many regions there will be in the hard days that come.
An example of an avenue with 5 skyscrapers after 2 days is given below.
</p>
<img src="/content/er2er:skyscrapers.png">

<h3>Input</h3>
<p>The input contains several test cases. The ﬁrst line contains an
integer <span style="font-style: italic;">t</span>
(t ≤ 15) denoting the number<br>
of test cases. Then <span style="font-style: italic;">t</span>
test cases follow. Each of them begins with a line containing two
numbers <span style="font-style: italic;">n</span>
and<br>
<span style="font-style: italic;">d</span> (1 ≤ n, d
≤ 10<sup>6</sup>), <span style="font-style: italic;">n</span>
is the number of skyscrapers and <span style="font-style: italic;">d</span>
is the number of days which the major wants<br>
to query. Skyscrapers are numbered from left to right. The next line
contains n integers h<sub>1</sub>, h<sub>2</sub>,
. . . , h<sub>n</sub><br>
where 1 ≤ h<sub>i</sub> ≤ 10<sup>9</sup> is the
height of skyscraper<span style="font-style: italic;"> i</span>.
The third line of a single test case contains <span style="font-style: italic;">d</span> numbers<br>
t<sub>j</sub> such that 0 ≤ t<sub>1</sub>
&lt; t<sub>2</sub> &lt; . . . &lt; t<sub>d−1</sub>
&lt; t<sub>d</sub> ≤ 10<sup>9</sup>.
</p>

<h3>Output</h3>
<p>For each test case output d numbers r<sub>1</sub>, r<sub>2</sub>,
. . . , r<sub>d</sub>, where r<sub>j</sub> is
the number of regions on day t<sub>j</sub> .
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
3 3
1 2 3
1 2 3
5 3
1 3 5 1 3
0 2 4


<b>Output:</b>
1 1 0
1 2 1
</pre>