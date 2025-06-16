<p>A positive integer <em>m</em>&nbsp;is called "self-descriptive" in base <em>b</em>, where <em>b</em>��2&nbsp;and <em>b</em> is an integer, if:</p>
<p>i) The representation of <em>m</em>&nbsp;in base <em>b</em> is of the form (a<sub>0</sub>a<sub>1</sub>...a<sub>b-1</sub>)<sub>b</sub></p>
<blockquote>
<p>(that is <em>m</em>=a<sub>0</sub>b<sup>b-1</sup>+a<sub>1</sub>b<sup>b-2</sup>+...+a<sub>b-2</sub>b+a<sub>b-1</sub>, where 0��a<sub>i</sub>��b-1 are integer)</p>
</blockquote>
<p>ii) a<sub>i</sub>&nbsp;is equal to the number of occurences of number i in the sequence (a<sub>0</sub>a<sub>1</sub>...a<span style="font-size: 8px;"><sub>b-1</sub></span>).</p>
<p>For example, (21200)<sub>5</sub>&nbsp;is "self-descriptive" in base 5, because it has five digits and contains two 0s, one 1s, two 2s, and no (3s and 4s).</p>
<p>(21200)<sub>5</sub>&nbsp;= (1425)<sub>10</sub>&nbsp;so 1425 is "self-descriptive" number.</p>
<p>Given <strong>n</strong>(1 �� <strong>n</strong> ��10<sup>18</sup>)and <strong>m</strong>&nbsp;(1 �� <strong>m</strong> �� 10<sup>9</sup>), your task is to find the <strong>n</strong>-th smallest "self-descriptive" number.</p>
<h3>Input</h3>
<p>The first line there is an integer <strong>T</strong>&nbsp;(1 �� <strong>T</strong>&nbsp;�� 10<sup>5</sup>).</p>
<p>For each test case there are two integers <strong>n</strong> and <strong>m</strong>&nbsp;written in one line, separated by a space.</p>
<h3>Output</h3>
<p>For each test case, output the <strong>n</strong>-th smallest "self-descriptive" number, (output the number in base 10) modulo <strong>m</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2</pre>
<pre>1 1000</pre>
<pre>2 1000

<strong>Output:</strong></pre>
<pre>100</pre>
<pre>136</pre>
<h3>Explanation</h3>
<p>100 is "self descriptive" number in base 4: (1210)<sub>4</sub></p>
<p>136 is "self descriptive" number in base 4: (2020)<sub>4</sub></p>
<p>&nbsp;</p>
<p><span style="color: #339966;"><span style="color: #339966;"><strong>Time limit ~230x My program speed:&nbsp;<a title="My Time" href="http://1.bp.blogspot.com/-Ij36hIcKmxU/UXzgbOvULwI/AAAAAAAAAUE/WjinW0h4PdM/s1600/SELFDESN.png" target="_blank">Click here to see my submission history and time record for this problem</a></strong></span></span></p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>