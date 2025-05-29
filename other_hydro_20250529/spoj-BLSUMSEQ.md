<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/BLSUMSEQ/en/">English</a></td>
<td width="50%"><a href="/problems/BLSUMSEQ/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given an positive integer n and a sequence a<sub>1</sub>…a<sub>n.</sub> There are q queries. Each query has one of two formats :</p>
<p><span style="white-space: pre;"> </span>- Format 0 l r k : you need to output the k-th smallest positive integer that can’t be partition into a sum of any subsequence of a<sub>l</sub>...a<sub>r&nbsp;</sub></p>
<p><span style="white-space: pre;"> </span>- Format 1 l r x : you need to output the numbers of ways to partition x into a sum of a subseqence of a<sub>l</sub>...a<sub>r</sub>&nbsp;(or the numbers of subsequence that sum of all its elements equal to x) (modulo 2<sup>32</sup>)</p>
<p><strong>Input :</strong></p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Fist line : two positive n and q (1 ≤ n ≤ 100, 1 ≤ q ≤ 10000)</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Second line : n positive a<sub>1</sub>…a<sub>n­&nbsp;</sub>(0 ≤ a<sub>i</sub>&nbsp;≤ 100)</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Next q lines : each line denotes a query with one of two format listed above (1 ≤ l ≤ r ≤ n, 1 ≤ k ≤ 10<sup>9</sup>, 0 ≤ x ≤ 10<sup>9</sup>)</p>
<p><strong>Output :</strong></p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; q lines : the i-th line is the answer of i-th query.</p>
<p><strong>Sample :</strong></p>
<p><strong><span style="white-space: pre;"> </span>Input :</strong></p>
<p><span style="white-space: pre;"> </span>5 3</p>
<p><span style="white-space:pre"> </span>1 0 2 4 1</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 200px; width: 1px; height: 1px; overflow: hidden;">0 2 3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 200px; width: 1px; height: 1px; overflow: hidden;">1 1 4 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 200px; width: 1px; height: 1px; overflow: hidden;">1 2 5 3</div>
<p><span style="white-space: pre;"> </span>0 2 3 2</p>
<p><span style="white-space: pre;"> </span>1 1 4 0</p>
<p><span style="white-space: pre;"> </span>1 2 5 3</p>
<p><strong><span style="white-space: pre;"> </span>Output :</strong></p>
<p><strong></strong><span style="white-space: pre;"> </span>3</p>
<p><span style="white-space: pre;"> </span>1</p>
<p><span style="white-space: pre;"> </span>2</p>
<p> </p>