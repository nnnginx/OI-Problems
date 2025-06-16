<p>You have a sack of <strong><span class="math"><em>n</em></span></strong> potatoes and a strip of land <strong><span class="math">(<em>n</em> + 1) ⋅ <em>k</em></span></strong> centimeters long.</p>
<p>You want to evenly plant the potatoes on this strip. If we mark the beginning of the strip as centimeter <span class="math">0</span>, then you want to plant the first potato at centimeter <strong><span class="math"><em>k</em></span></strong>, plant the second potato at centimeter <strong><span class="math">2<em>k</em></span></strong>, <span class="math">...</span>, plant the <strong><span class="math"><em>n</em></span></strong>-th potato at centimeter <strong><span class="math"><em>n</em><em>k</em></span></strong> (and then the strip of land ends at <strong><span class="math">(<em>n</em> + 1) ⋅ <em>k</em></span></strong> centimeters).</p>
<p>Each potato has a growth range <strong><span class="math"><em>r</em><sub><em>i</em></sub></span></strong>. This means that if you plant the potato at centimeter <strong><span class="math"><em>x</em></span></strong>, and it has enough space, it will grow you some new tasty potatoes all across<strong> <span class="math">[<em>x</em> − <em>r</em><sub><em>i</em></sub>, <em>x</em> + <em>r</em><sub><em>i</em></sub>]</span></strong>.</p>
<p>However, a potato will never grow over another potato's growth territory, or beyond your strip of land - in other words, if the potato comes across the edge of the plot or bumps into a different potato plant, it stops growing in that direction.</p>
<p>Given <strong><span class="math"><em>n</em></span></strong>, <strong><span class="math"><em>k</em></span></strong> and <strong><span class="math"><em>r</em><sub><em>i</em></sub></span></strong> of your <strong><span class="math"><em>n</em></span></strong> potatoes, how many potatoes can you grow if you plant them optimally?</p>
<h3 id="input">Input</h3>
<p>The first line contains an integer <strong><span class="math">1 ≤ <em>T</em> ≤ 20</span> </strong>- the number of test cases. <strong><span class="math"><em>T</em></span> </strong>test cases follow.</p>
<p>For each test case:</p>
<p>The first line contains the integers <strong><span class="math">1 ≤ <em>n</em> ≤ 10<sup>6</sup></span></strong> and <strong><span class="math">1 ≤ <em>k</em> ≤ 10<sup>9</sup></span></strong>. The second line contains <strong><span class="math"><em>n</em></span></strong> integers <strong><span class="math">1 ≤ <em>r</em><sub><em>i</em></sub> ≤ <em>k</em></span></strong> - the growth radii of the potatoes.</p>
<p>The sum of <strong><span class="math"><em>n</em></span></strong> within an input file will never exceed <strong><span class="math">2 ⋅ 10<sup>6</sup></span></strong>.</p>
<h3 id="output">Output</h3>
<p>For each test case, output a single integer: the maximum length of strip you can cover in grown potatoes.</p>
<h3 id="examples">Examples</h3>
<p><strong>Input</strong></p>
<pre><code>3
3 20
6 12 4
3 20
12 12 12
3 5
1 1 5</code></pre>
<p><strong>Output</strong></p>
<pre><code>44
64
13</code></pre>
<p><em>In the first case, if we plant the potatoes in the same order as in the input, that is 6-&gt;20cm, 12-&gt;40cm, 4-&gt;60cm, they will grow on [14,26], [28,52], [56,64] for a total of 12+24+8 = 44 cm of potatoes. Any other order works just as well, though.</em></p>
<p><em>In the second case we don't really have much to choose from.. The potatoes would want to grow out to [8,32], [28,52], [48,72], but they get in each other's way. So they will end up growing on [8,30], [30,50], [50,72] for a total of 64cm.</em></p>
<p><em>In the last case the best order to plant the potatoes is, for example, 5 1 1</em>.</p>