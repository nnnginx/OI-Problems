<p>Eagle (AKA Mohamed Ahmed) lives in a city consists of <strong>n</strong> intersections connected by n-1 roads, in a way that can go from any intersection to any other intersection moving along some of these roads.</p>
<p>Every day he starts walking in the city following a simple strategy; if he's at some intersection he <strong>has to </strong>pick one of the roads connected to it at random such that he hasn't walked through it before and walk through it and and if there isn't any, he stops and goes home.</p>
<p>His only problem is that he's afraid of dogs. He doesn't even like seeing dogs. So he's wondering in the worst scenario, how many dogs he'll have to see during his walk until he stops if he starts walking at some intersection. Can you help him?</p>
<h3>Input</h3>
<p>The input starts with an integer <strong>T</strong> (1 &lt;= <strong>T</strong> &lt;= 10), the number of test cases. following T blocks describing each test case.</p>
<p>Each block starts with a line containing an integer <strong>n</strong> (2 &lt;= <strong>n</strong> &lt;= 10<sup>5</sup>), the number of intersections in the city. Intersections are numbers 1 through n.</p>
<p>Followed by n-1 lines each containing integers u, v, (1 &lt;= u, v &lt;= n) and <strong>d</strong> (1 &lt;= <strong>d</strong> &lt;= 10<sup>9</sup>), the numbers of intersections at the end of this road and the number od dogs Eagle will see walking in this road.</p>
<h3>Output</h3>
<p>For each test case print a line containing n integers, the <em>i</em>th integer represents the maximum number of dogs Eagle might see if he starts his walk at intersection <em>i</em>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>4<br>1 2 3<br>3 2 4<br>3 4 5</pre>
<pre><strong>Output:</strong>
12 9 7 12
</pre>