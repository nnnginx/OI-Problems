<p>You are given <strong>n</strong> numbers initially. You have to maintain a <strong>multiset</strong> for those <strong>n</strong> numbers. Then you are given <strong>q</strong> queries. Qeuries will be one of the following types -</p>
<p>1) <strong>1 x</strong> : Let <strong>a</strong> be the count of elements smaller than or equal to <strong>x</strong>. Add <strong>x+a</strong> into the multiset.&nbsp;</p>
<p>2) <strong>2 y</strong> : report the number of numbers in the multiset that are smaller than or equal to <strong>y</strong>.</p>
<p>3) <strong><strong>3 z</strong></strong> : report the <strong>z</strong>th smallest number of the multiset. Note that if any number <strong>d</strong> appears more than once, it is to be counted as many times it appears! Also, if z exceeds the number of elements in the <strong>multiset</strong>, that is answer for this query doesn't exist, print "<strong>invalid". </strong>Look at the sample input for clarification.</p>
<h3>Note:</h3>
<p><em><span style="font-weight: normal;">since it is a </span><span style="font-weight: normal;"><strong>multiset</strong></span><span style="font-weight: normal;">, it will also store duplicates. Also, lets say our multiset has elements 1,2,2,3,3,3. then for z=3, answer would be </span><span style="font-weight: normal;"><strong>2 .</strong></span></em></p>
<p><span style="font-weight: normal;"><strong>Constraints&nbsp;</strong></span></p>
<p><strong>1&lt;=n&lt;=100000</strong></p>
<p><strong>1&lt;=q&lt;=100000</strong></p>
<p><strong>1&lt;=x&lt;=(10^9-2*10^5)</strong></p>
<p><strong>1&lt;=y,z&lt;=10^9</strong></p>
<p><strong>1&lt;=Initial elements of the multiset&lt;=</strong><span style="font-weight: bold;">(10^9-2*10^5)</span></p>
<h3>Input</h3>
<p>The first line &nbsp;will contain two integers, n and q, denoting the number of initially members of the multiset and the number of queries.</p>
<p>Next q lines will be of he form -&nbsp;</p>
<p><strong>Type D : </strong>That is, the queries will be of the one of given 3 types and accordingly, you will be given and integer D.</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">10 20</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">7 35 44 25 15 10 21 42 12 33&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 39</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">2 47</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">2 96</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 29</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">2 40</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">3 27</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">3 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 22</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 44</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">3 32</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 28</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">2 39</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">3 23</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">2 31</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 13</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">1 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">3 38</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 152.727px; width: 1px; height: 1px; overflow: hidden;">2 26</div>
<p>&nbsp;</p>
<h3>Output</h3>
<p>You have to print the output for query numbers <strong>2</strong> and <strong>3.</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p style="white-space: normal;">10 20</p><p style="white-space: normal;">7 35 44 25 15 10 21 42 12 33&nbsp;</p><p style="white-space: normal;">1 6</p><p style="white-space: normal;">1 39</p><p style="white-space: normal;">2 47</p><p style="white-space: normal;">2 96</p><p style="white-space: normal;">1 29</p><p style="white-space: normal;">2 40</p><p style="white-space: normal;">3 27</p><p style="white-space: normal;">3 5</p><p style="white-space: normal;">1 22</p><p style="white-space: normal;">1 44</p><p style="white-space: normal;">3 32</p><p style="white-space: normal;">1 28</p><p style="white-space: normal;">3 2</p><p style="white-space: normal;">2 39</p><p style="white-space: normal;">3 23</p><p style="white-space: normal;">2 31</p><p style="white-space: normal;">1 13</p><p style="white-space: normal;">1 50</p><p style="white-space: normal;">3 38</p><p style="white-space: normal;">2 26</p>

<strong>Output:</strong>
<p style="white-space: normal;">11</p><p style="white-space: normal;">12</p><p style="white-space: normal;">10</p><p style="white-space: normal;">invalid</p><p style="white-space: normal;">15</p><p style="white-space: normal;">invalid</p><p style="white-space: normal;">7</p><p style="white-space: normal;">12</p><p style="white-space: normal;">invalid</p><p style="white-space: normal;">8</p><p style="white-space: normal;">invalid</p><p style="white-space: normal;">8</p>
</pre>