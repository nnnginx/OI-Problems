<div>
<p>There are <span><em>x</em></span> villages in Andhere Nagar. Each village has its index — an integer number from <span>1</span> to <span><em>x</em></span>. The capital has index <span>a</span>.  All the roads in Andhere Nagar are two-way. The road system is such that  there is exactly one path from the capital to each city, i.e. the road  map looks like a tree. In Andhere Nagar's chronicles the road map is kept in  the following way: for each village <span><em>i</em></span>, different from the capital, there is kept number <span><em>p</em><sub><em>i</em></sub></span> — index of the last village on the way from the capital to <span><em>i</em></span>.</p>
<p>Once the king of Andhere Nagar, Choupat Raja, decided to move the capital from village <span>a</span> to village<span> b</span>.  Naturally, after this the old representation of the road map in Andhere Nagar 's chronicles became incorrect. Please, help the king find out a  new representation of the road map in the way described above.</p>
</div>
<h3>Input</h3>
<p>The first line contains three space-separated integers <span><em>x</em></span>, <span>a</span>, <span>b</span> (<span>2 ≤ <em>x</em> ≤ 5· 10<sup>4</sup>, 1 ≤ a ≠ b ≤ <em>n</em></span>) — amount of villages in Andhere Nagar, index of the old capital and index of the new one, correspondingly.</p>
<p>The following line contains <span><em>x</em> - 1</span> space-separated integers — the old representation of the road map. For each city, apart from <span>a</span>, there is given integer <span><em>p</em><sub><em>i</em></sub></span> — index of the last city on the way from the capital to city <span><em>i</em></span>. All the cities are described in order of increasing indexes.</p>
<h3>Output</h3>
<p>Output <span><em>x</em> - 1</span> numbers — new representation of the road map in the same format.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong><br>3 2 3<pre>2 2</pre>
<br><strong>Output:</strong><br>2 3 <br></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong><br>6 2 4<pre>6 1 2 4 2</pre>
<br><strong>Output:</strong><br>6 4 1 4 2<br><br></pre>