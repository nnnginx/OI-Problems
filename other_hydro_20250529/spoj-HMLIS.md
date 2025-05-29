<p>The task is simply to find LIS and number of way we can select distinct LIS</p>
<p>Definition :</p>
<p>LIS (short for Longest Increasing Subsequence) is the longest subsequence of the sequence in which every element in the subsequence is increasing.</p>
<p>an LIS is distinct when one of the element come from different index of the beginning array.</p>
<p>this task involve finding length of Longest IS and number of way LIS can be made.</p>
<h3>Input</h3>
<p>First line : integer <em><strong>N</strong> </em>represent number of elements in the sequence <strong><em>N &lt;= 100000</em></strong></p>
<p>Second line :<strong><em> N</em></strong> integers represent number in the sequence, each integer is in the range [1, 100000000]</p>
<h3>Output</h3>
<p>2 integer in 1 line, Lenght of LIS and Number of LIS that can be made.</p>
<p>The ans can be very large, so print both ans mod 1000000007</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>5
1 3 2 5 4</p>
<strong>Output:</strong>
<p>3 4
// Explanation : the subsequence are
// (1, 3, 5), (1, 3, 4), (1, 2, 5), (1, 2, 4)</p><p>&nbsp;</p>
</pre>
<pre><strong>Input:</strong>
<p>5
1 2 5 3 3</p>
<strong>Output:</strong>
<p>3 3
// Explanation : the subsequence are
// (1, 2, 5), (1, 2, 3), (1, 2, 3)
// note that there're two <span style="text-decoration: underline;">3</span> in the sequence which count seprerately.</p>
</pre>