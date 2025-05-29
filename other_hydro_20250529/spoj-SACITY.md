<p><span style="font-size: small;">Sadde owns a country named as Sadde land. In Sadde land each city consists of only one row of building.</span></p>
<p><span style="font-size: small;">Sadde being the king wanted to know the score of cities in his country. Sadde gives the task of scoring to one of his minister Dukker.</span></p>
<p><span style="font-size: small;">Each city consists of ¡°N¡± buildings in a single row and each building is having a container in front of them. For each building in the city Dukker calculate the number of buildings having less height in left of that building(say <strong>Hmin<sub>i</sub></strong>) and number of buldings having <span style="font-size: small;">greater&nbsp;</span>height in right of that building(say <strong>Hmax<sub>i</sub></strong>). He put <strong>Hmin<sub>i</sub>&nbsp;+ Hmax<sub>i</sub></strong>&nbsp;number of flags in container of <strong>i<sup>th</sup>&nbsp;</strong>building.</span></p>
<p><span style="font-size: small;">He took all containers from the buildings and shuffles them. Now he wants to distribute flags among buildings of city such that each building should get same number of flag and a building will get all the flags from single container.</span></p>
<p><span style="font-size: small;">Score of city is the maximum number of flags that a building can have.</span></p>
<h3>Input</h3>
<p><span style="font-size: small;">Input consist of <strong>T</strong>&nbsp;number of test cases. Each case contains two lines.&nbsp; First line contains <strong>N</strong><strong>&nbsp;</strong>denoting number of building in a city. Second line will contain <strong>N</strong> integers denoting <strong>H</strong><sub>i</sub>(height of building).</span>&nbsp;</p>
<h3>Constrains</h3>
<p><strong>T</strong><span style="font-size: small;">&lt;=10</span></p>
<p><span style="font-size: small;">0 &lt;&nbsp;<strong>N </strong><span style="font-size: small;">&lt;= 10<sup>5</sup></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">0 &lt;= <strong>H</strong><sub>i</sub><span style="font-weight: bold;">&nbsp;&lt;= 10<sup>9</sup></span></span></span></p>
<h3>Output</h3>
<p><span style="font-size: small;">Output should contain <strong>T</strong> line denoting score of that city.</span></p>
<h3>Example</h3>
<pre><span style="font-size: medium;"><strong>Input:</strong>
<strong>3</strong></span></pre>
<pre><strong><span style="font-size: medium;">5</span></strong></pre>
<pre><strong><span style="font-size: medium;">1 2 3 4 5</span></strong></pre>
<pre><strong><span style="font-size: medium;">5</span></strong></pre>
<pre><strong><span style="font-size: medium;">4 2 5 3 1</span></strong></pre>
<pre><strong><span style="font-size: medium;">3</span></strong></pre>
<pre><span style="font-size: medium;"><strong>3 3 3
</strong>
<strong>Output:</strong>
4</span></pre>
<pre><span style="font-size: medium;">1</span></pre>
<pre><span style="font-size: medium;">0</span></pre>