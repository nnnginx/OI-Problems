<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Harry's friend Charlie Weasley has partnered with an old-time breeder of dragons in Romania. &nbsp;When Harry visited Charlie over the summer, Charlie showed him breeding records stretching back centuries. &nbsp;It had started out with just one female dragon named Abraxia that had then reproduced to give many generations of dragons. &nbsp;The breeding record showed a family tree of dragons, starting with Abraxia and showing each descendant* (only females' descendants were shown), &nbsp;the year each was hatched from its egg and the year each died. &nbsp;Only already dead dragons were included. Charlie pointed out that a dragon matured early, and once hatched, could herself lay and hatch an egg in the very year it was born. &nbsp;Dragon eggs did not need a mother's care to hatch -- the breeders simply used the warmth of a blowtorch to keep the egg warm and hatch it, sometimes long after the mother dragon was dead.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Harry noticed that sometimes many generations of dragons were alive at the same time. &nbsp; He was curious to figure out, for each dragon when it was alive, what was the maximum generational difference (absolute value) between it and its coeval** descendants. &nbsp;Can you help him? &nbsp;Assume that if a dragon dies the year another is hatched, they were coeval.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">*A descendant is a child, grandchild, great-grandchild etc.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">**coeval: Alive at the same time.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line of each test case starts with an integer N - the number of dragons.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">It is followed by N lines. The ith line (0 indexed) contains 3 integers, p_i, hatchyear_i and deathyear_i. p_i is the parent of ith dragon and its interval is hatchyear_i to deathyear_i. &nbsp;The dragon with index 0 is Abraxia, and a mother's index is smaller than all its descendants'.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each line contains a space-separated list of N integers, the ith of them denoting the required answer for the ith dragon. If the ith dragon's life does not overlap with any descendant's, output 0 for that dragon.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= N &lt;= 70000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 &lt;= hatchyear &lt;= deathyear &lt;= 10^9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">p_0 = -1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For all i &gt; 0, 0 &lt;= p_i &lt; i</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">hatchyear of dragon &gt;= hatchyear of its mother</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit: 3s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit: 64 MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">-1 0 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 1 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 2 8</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 2 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 10 12</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">-1 0 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 1 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 2 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 2 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">6 10 11</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">6 20 30</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 0 0 0 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 0 1 0 0 0 0 0 0</div>
<p>&nbsp;</p>
<p>Harry's friend Charlie Weasley has partnered with an old-time breeder of dragons in Romania. &nbsp;When Harry visited Charlie over the summer, Charlie showed him breeding records stretching back centuries. &nbsp;It had started out with just one female dragon named Abraxia that had then reproduced to give many generations of dragons. &nbsp;The breeding record showed a family tree of dragons, starting with Abraxia and showing each descendant* (only females' descendants were shown), &nbsp;the year each was hatched from its egg and the year each died. &nbsp;Only already dead dragons were included. Charlie pointed out that a dragon matured early, and once hatched, could herself lay and hatch an egg in the very year it was born. &nbsp;Dragon eggs did not need a mother's care to hatch -- the breeders simply used the warmth of a blowtorch to keep the egg warm and hatch it, sometimes long after the mother dragon was dead.</p>
<p>Harry noticed that sometimes many generations of dragons were alive at the same time. &nbsp; He was curious to figure out, for each dragon when it was alive, what was the maximum generational difference (absolute value) between it and its coeval** descendants. &nbsp;Can you help him? &nbsp;Assume that if a dragon dies the year another is hatched, they were coeval.</p>
<p>&nbsp;</p>
<p>*A descendant is a child, grandchild, great-grandchild etc.</p>
<p>**coeval: Alive at the same time.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test cases T.</p>
<p>The first line of each test case starts with an integer N - the number of dragons.</p>
<p>It is followed by N lines. The ith line (0 indexed) contains 3 integers, p_i, hatchyear_i and deathyear_i. p_i is the parent of ith dragon and its interval is hatchyear_i to deathyear_i. &nbsp;The dragon with index 0 is Abraxia, and a mother's index is smaller than all its descendants'.&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output T lines.</p>
<p>Each line contains a space-separated list of N integers, the ith of them denoting the required answer for the ith dragon. If the ith dragon's life does not overlap with any descendant's, output 0 for that dragon.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 3</p>
<p>1 &lt;= N &lt;= 70000</p>
<p>0 &lt;= hatchyear &lt;= deathyear &lt;= 10^9</p>
<p>p_0 = -1</p>
<p>For all i &gt; 0, 0 &lt;= p_i &lt; i</p>
<p>hatchyear of dragon &gt;= hatchyear of its mother</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>5</p>
<p>-1 0 10</p>
<p>0 1 5</p>
<p>0 2 8</p>
<p>0 2 5</p>
<p>3 10 12</p>
<p>9</p>
<p>-1 0 10</p>
<p>0 1 1</p>
<p>0 2 2</p>
<p>1 2 3</p>
<p>1 3 4</p>
<p>2 2 3</p>
<p>2 2 4</p>
<p>6 10 11</p>
<p>6 20 30</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2 0 0 0 0</p>
<p>3 0 1 0 0 0 0 0 0</p>
<p>&nbsp;</p>
<p>&nbsp;</p>