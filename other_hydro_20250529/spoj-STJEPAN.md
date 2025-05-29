<p>&nbsp;</p>
<p>Little Stjepan lives in a village which can be represented as X-axis. In village there are N beer machines, machine i has x coordinate P<sub>i</sub> and needs T<sub>i</sub> seconds to produce 1 liter of beer.</p>
<p>This year M tourists (one by one because there is only one guide, Stjepan) will visit his village, tourist i will arrive at point A<sub>i</sub>, want to drink L<sub>i</sub> liters of beer but will have energy to walk at most D<sub>i</sub> seconds (that is D<sub>i</sub> units of length), he will walk to beer machine Stjepan suggests him and as soon as machine produces L<sub>i</sub> liters of beer tourist will be able to enjoy it.</p>
<p>As Stjepan wants all tourists to come next year too he will choose machine for each tourist so that tourist can get a beer as soon as possible. Help Stjepan to do that and write program which will output minimal sum of passed times from arrival of tourist to getting a beer. If a tourist can't get a beer then his time is 0.</p>
<p>Note that tourists are independent and machines can be used multiple times.</p>
<h3>Input</h3>
<p>On first line of standard input you are given two integers (2 �� N �� 250 000, 1 �� M �� 500 000), number of beer machines and number of tourists.</p>
<p>Next 5 lines contain 4 integers (X<sub>0</sub>, A, B, C) each and they describe arrays P, T, A, L and D, respectively.<br>With these four numbers i-th element of array is defined as X<sub>i</sub> = 1 + ((X<sub>i-1</sub>*A + B) mod C), where indices are 1-based and X<sub>0</sub> is given in input.</p>
<p>1 �� X<sub>0</sub>, A, B, C&nbsp;��&nbsp;10<sup>9</sup>.</p>
<p><strong>Note:</strong>&nbsp;Author's solution doesn't depend on properties of pseudo-random generator.</p>
<h3 style="font-size: 1.17em;">Output</h3>
<p>Output total time from task statement.&nbsp;Answer will fit in 64-bit signed integer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 302px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 4</div>3 4
1 4 3 6
2 4 4 10
3 8 1 10
3 1 8 7
1 3 2 6
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 302px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 3 2</div>
<strong>Output:</strong>
53</pre>
<pre><span style="white-space: normal; font-size: 12px; color: #181818; line-height: 18px;"><span style="color: #000000;"><strong>Explanation</strong></span><span class="sy4"><span style="color: #000000;"><strong>:</strong></span></span><span style="color: #000000;">&nbsp;<br>Machines (P, T) : (2, 3), (6, 7), (4, 3)<br></span></span><span style="white-space: normal; font-size: 12px; line-height: 18px;">Tourists (A, L, D) : (6, 5, 6), (10, 7, 3), (2, 2, 6), (8, 4, 3)</span></pre>
<pre><span style="white-space: normal; font-size: 12px; color: #181818; line-height: 18px;"><span style="color: #000000;">Tourist&nbsp;</span><span class="co2"><span style="color: #000000;">#1 -&gt; Machine #3 -&gt; 17 time units<br></span></span></span><span style="white-space: normal; font-size: 12px; line-height: 18px;">Tourist #2 -&gt; No beer :( -&gt; 0 time units<br>Tourist #3 -&gt; Machine #1 -&gt; 6 time units<br>Tourist #4 -&gt; Machine #2 -&gt; 30 time units</span></pre>