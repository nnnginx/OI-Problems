<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/CARDSHUF/en/">English</a></td>
<td width="50%"><a href="/problems/CARDSHUF/vn/">Tiếng Việt</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>"Phú ông" has a card deck consits of n cards. He writes on each card a number from 1 to n from the top to the bottom of the deck. <br> Then he does shuffle the card deck several times, each time is described by <strong>S(i, j)</strong> meaning: pull out the i<sup>th</sup> card then put it on the j<sup>th</sup> of the remaining cards (1 ≤ i, j ≤ n). If j = n, the i<sup>th</sup> card will be the bottom card of the new one. <br> For example (<strong>n=6</strong>): <br> <img src="../../../content/anhdq:cardshuf_sample.jpg" alt=""> <br> Afer x times of shuffing, "Phú ông" gives "Bờm" the card deck and chanllenges him to make it into the original order. Please help "Bờm"!</p>
<h3>Input</h3>
<p>- The first line contains two integer n, x. <br> - Next x line(s), the p<sup>th</sup> line contains two integer i<sub>p</sub>, j<sub>p</sub> describing the p<sup>th</sup> time of shuffing (<strong>S(i<sub>p</sub>, j<sub>p</sub>)</strong>).</p>
<h3>Output</h3>
<p>- A single integer means the minimal number of times of shuffing the card deck to help "Bờm".</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>6 4<br>2 3<br>1 2<br>4 5<br>1 6<br><br><strong>Output:</strong><br>2<br></pre>
<h3>Limitations</h3>
<p>- 1 ≤ n, x ≤ 10<sup>5</sup>.</p>
<p></p>