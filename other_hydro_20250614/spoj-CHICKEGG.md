<p>There are n hens in a farm. The egg hatching ability of all the hens decreases by 1 day after each time they hatch an egg. (i.e. every hen will hatch the next egg 1 day slower than the time it took to hatch the previous egg)</p>
<p>Let the initial egg hatching ability of Hen[i] be D[i].</p>
<ul>
<li>Hen[i] lays it's first egg on D[i]th day.</li>
<li>Hen[i] lays it's second egg on 2*D[i]+1 th day.</li>
<li>Hen[i] lays it's thrid egg on 3*D[i]+3rd day.</li>
<li>Hen[i] lays it's fourth egg on 4*D[i]+6th day.</li>
<li>Hen[i] lays it's fifth egg on 5*D[i]+10th day.</li>
</ul>
<p>and so on..</p>
<p>&nbsp;</p>
<p>Given <strong>n</strong> - the number of hens and the array <strong>D</strong> - the initial egg hatching ability of the hens, find the minimum number of days required to produce at least <strong>K</strong> eggs. You can safely assume that eggs neither gets damaged nor converted into hens.</p>
<h3>Input</h3>
<p>The first line consists of integers <strong>t</strong>, the number of test cases. For each test case, the first line consists two integers <strong>n</strong> and <strong>K</strong>. The next line consists of <strong>n</strong> integers representing the initial egg hatching ability of the hens.</p>
<h3>Output</h3>
<p>For each test case, find the minimum number of days required to produce at least <strong>K</strong> eggs.</p>
<h3>Constraints</h3>
<p>1 &lt;= t &lt;= 10^2<br> 1 &lt;= n &lt;= 10^3<br> 1 &lt;= K &lt;= 10^8<br> 1 &lt;= D[i] &lt;= 10^8</p>
<h3>Example</h3>
<pre><strong>Sample Input:</strong>
3
1 4
1
2 5
2 5
5 1000000
1 2 3 4 5

<strong>Sample Output:</strong>
10
11
20000500003</pre>
<h3>Explanation of Test case #2</h3>
<p>There are 2 hens and we need to produce 5 eggs</p>
<p>At time 2, Hen 0 lays an egg.</p>
<p>At time 5, Hen 0 and Hen1 lay an egg each.</p>
<p>At time 9, Hen 0 lays an egg</p>
<p>At time 11, Hen1 lays an egg.</p>