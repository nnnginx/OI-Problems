<p style="text-align: justify;">Oňo the grasshopper wants to cross the river. But the river is very wide – <strong><span class="math inline"><em>w</em></span></strong> meters from one bank to the other, and Oňo can only jump up to <strong><span class="math inline"><em>d</em></span></strong> meters at once. Fortunately, there are <strong><span class="math inline"><em>n</em></span></strong> lily pads growing in the river. They’re not big enough yet, but once they are adult, they will be able to hold Oňo’s weight.</p>
<p style="text-align: justify;">The <strong><span class="math inline"><em>i</em></span></strong>-th lily pad is located <strong><span class="math inline"><em>m</em><sub><em>i</em></sub></span></strong> meters away from the left bank, where Oňo is right now. It will become able to support Oňo <strong><span class="math inline"><em>s</em><sub><em>i</em></sub></span></strong> seconds from now. But <strong><span class="math inline"><em>e</em><sub><em>i</em></sub></span></strong> seconds from now it will become too old and die.</p>
<p style="text-align: justify;">Oňo is very fast and he can perform multiple jumps (each up to <strong><span class="math inline"><em>d</em></span></strong> meters) in a single second – every jump is practically instant. But he is still nervous. If he doesn’t plan things through, he could end up jumping across some lily pads only to find out there is no way forward, and now the lily pads behind him are gone and he can’t even get back! Oh, the horror! To prevent this, Oňo will only jump across the lily pads when he can immediately get from one side of the river to the other without stopping.</p>
<p style="text-align: justify;">It would be great if someone wrote a program telling him at what time he can do so, and the total time that the river is crossable.</p>
<h4 id="task-english" style="text-align: justify;">Task</h4>
<p style="text-align: justify;">Each lily pad has a time <strong><span class="math inline"><em>s</em><sub><em>i</em></sub></span></strong> when it turns adult and a time <strong><span class="math inline"><em>e</em><sub><em>i</em></sub></span></strong> when it dies; it can hold Oňo from the <strong><span class="math inline"><em>s</em><sub><em>i</em></sub></span></strong>-th to the <strong><span class="math inline"><em>e</em><sub><em>i</em></sub></span></strong>-th second. The lily pad is located <strong><span class="math inline"><em>m</em><sub><em>i</em></sub></span></strong> meters from the left bank of the river.</p>
<p style="text-align: justify;">Find the earliest time that Oňo can cross the river without stopping, and also how many seconds there are such that he is able to do so.</p>
<p>Note that Oňo is not brave enough to jump from a lily pad which grows old at time <strong><span class="math inline"><em>t</em></span></strong> to a lily pad which becomes adult at the same time <strong><span class="math inline"><em>t</em></span></strong> - in other words, you may imagine that at the beginning of each second, first the appropriate lily pads die and then the appropriate lily pads become adult.</p>
<h4 id="input-english" style="text-align: justify;">Input</h4>
<p style="text-align: justify;">The first line contains an integer <strong>1 ≤ T ≤ 3</strong> - the number of test cases. The only input file with <strong>T &gt; 1</strong> is the sample shown below.</p>
<p style="text-align: justify;"><strong>T</strong> test cases follow, each ends with a blank line.</p>
<p style="text-align: justify;">The first line contains three integers <strong><span class="math inline"><em>n</em></span></strong>, <strong><span class="math inline"><em>w</em></span></strong> and <strong><span class="math inline"><em>d</em></span></strong> - the number of lily pads, the width of the river, and Oňo’s jump distance, where <strong><span class="math inline">1 ≤ <em>n</em> ≤ 500 000</span></strong> and <strong><span class="math inline">1 ≤ <em>d</em> &lt; <em>w</em> ≤ 10<sup>9</sup></span></strong>.</p>
<p style="text-align: justify;"><strong><span class="math inline"><em>n</em></span></strong> lines will follow, each containing three integers <span class="math inline"><strong><em>m</em><sub><em>i</em></sub>&nbsp;<em>s</em><sub><em>i</em></sub>&nbsp;<em>e</em></strong><sub><em>i</em></sub></span> describing one lily pad: its distance in meters from the left bank, the time it turns adult, and the time it grows old. <strong><span class="math inline">0 &lt; <em>m</em><sub><em>i</em></sub> &lt; <em>w</em></span></strong> and <strong><span class="math inline">1 ≤ <em>s</em><sub><em>i</em></sub> &lt; <em>e</em><sub><em>i</em></sub> ≤ 10<sup>15</sup></span></strong>.</p>
<p style="text-align: justify;">No two lily pads with the same position <strong><span class="math inline"><em>m</em><sub><em>i</em></sub></span></strong> will be alive at the same time, in particular if any two lily pads have the same <strong>m<sub>i</sub></strong>, one will die at least a second before the other becomes adult.</p>
<h4 id="output-english" style="text-align: justify;">Output</h4>
<p style="text-align: justify;">For each test case, output two integers <strong><span class="math inline"><em>e</em></span></strong> and <strong><span class="math inline"><em>t</em></span></strong> in a single line, where <strong><span class="math inline"><em>e</em></span></strong> is the earliest time at which Oňo can jump all the way from the left to the right bank of the river without stopping, and <strong><span class="math inline"><em>t</em></span></strong> is the total number of seconds during which he can do so (not necessarily continuously from <strong><span class="math inline"><em>e</em></span></strong>).</p>
<p style="text-align: justify;">If Oňo can never cross the river, print <strong><span class="math inline"><em>e</em></span></strong> as <span class="math inline">−1</span>.</p>
<h4 id="examples" style="text-align: justify;">Examples</h4>
<p style="text-align: justify;"><strong>Input:</strong></p>
<pre style="text-align: justify;"><code>3
7 60 10
10 1 10
20 1 7
20 8 11
40 1 20
50 4 15
30 5 12
30 1 3

2 100 80
1 1 5
81 5 123

20 5 1
1 1 189
2 1 2
3 1 2
4 1 2
2 109 189
3 109 189
4 109 323
1 281 462
2 281 323
3 281 323
2 337 743
3 337 462
4 337 462
1 616 743
3 616 743
4 616 1016
1 874 1327
2 874 1327
3 874 1327
4 1163 1327
</code></pre>
<p style="text-align: justify;">Output:</p>
<pre style="text-align: justify;"><code>5 4
-1 0
1 681</code></pre>
<p style="text-align: justify;"><em>In the first case, at time 5, the first, second, fourth, fifth, and sixth lillies are alive, and Oňo can jump across. He can do so until the 7th second for a total of 2 seconds, when the second lily pad dies, then again from the 8th second to the 10th second, after which the first lily pad dies and the river becomes uncrossable forever.</em></p>
<p style="text-align: justify;"><em>In the second case the lily pads just barely miss themselves, and Oňo can never get across.</em></p>