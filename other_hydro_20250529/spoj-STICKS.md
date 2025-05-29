<p><span style="font-size: small;">We have N sticks are lined up in a queue with different distances between them , and each stick is leaning on the left stick (look at figure) .</span></p>
<p><span style="font-size: small;">L : the length of the stick.</span></p>
<p><span style="font-size: small;">D : the distance between the stick head point and the left one head point.</span></p>
<p><span style="font-size: small;"><img src="../../../content/simes:Sticks.png" alt="" width="257" height="196"></span></p>
<p><span style="font-size: small;">We catch the first stick (that length L0) <span id="result_box" lang="en">and keep it vertical.</span></span></p>
<p><span style="font-size: small;">determine <span id="result_box" lang="en">the total time that </span>expected<span id="result_box" lang="en"> to</span> fall down all sticks<span id="result_box" lang="en"> if the first stick moved away (assume that each stick's </span>bottom head will not displaced , and when the stick reach ground it will vanish and the right one start to fall ).</span></p>
<p><span style="font-size: small;">you will have V (</span><span style="font-size: small;">linear velocity for the head point</span><span style="font-size: small;">) at time = 1 second (from the stick start to fall , if we assume that stick will not stop and keeping same motion type).</span></p>
<p><span style="font-size: medium;">suppose that wight force has stable effect on the stick in dirction and value</span></p>
<p>&nbsp;</p>
<h3>Input</h3>
<p><span style="font-size: small;">the first line : N , L0</span></p>
<p><span style="font-size: small;">next N-1 Line : L<span style="font-family: courier new,courier;">k</span> , D<span style="font-family: courier new,courier;">k</span> , V<span style="font-family: courier new,courier;">k</span>(1)</span></p>
<h3>Output</h3>
<p><span style="font-size: small;">One number T (total time in millisecond). </span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 8.75<br>10 8.7 25000

<strong>Output:</strong>
2
<br><br><br><br><span style="font-size: medium;">2 &lt;= N &lt;= 5000<br></span><span style="font-size: medium;">1 &lt;= L &lt;= 1000000</span><br><span style="font-size: medium;">1 &lt;= V &lt;= 1000000</span><br><br>.</pre>