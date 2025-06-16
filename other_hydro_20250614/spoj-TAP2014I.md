<p><strong>[ The original version of this problem (in Spanish) can be found at <a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a>&nbsp;]</strong></p>
<p>Two natural numbers <strong>n</strong> and <strong>m</strong> are said to be <em>coprime</em> if their greatest common divisor is the number <strong>1</strong>. In other words, <strong>n</strong> and <strong>m</strong> are coprime if there is no integer <strong>d &gt; 1</strong> such that <strong>d</strong> exactly divides both <strong>n</strong> and <strong>m</strong>. A finite set of two or more consecutive natural numbers is called a "<em>stapled interval</em>" if there is no number in it that is coprime to all other numbers in the set.</p>
<p>Given a range <strong>[A, B]</strong>, we would like to count the number of stapled intervals completely contained in it. I.e., we want to know how many different pairs <strong>(a, b)</strong> exist such that <strong>A ��&nbsp;a &lt; b&nbsp;��&nbsp;B</strong> and the set <strong>{a, a+1, ..., b}</strong> is a stapled interval.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>P</strong> representing the number of questions you should answer (<strong>1&nbsp;</strong><span style="font-weight: bold;">��</span><strong>&nbsp;P&nbsp;</strong><span style="font-weight: bold;">��</span><strong>&nbsp;1000</strong>). Each of the following <strong>P</strong> lines describes a question, and contains two integer numbers <strong>A</strong> and <strong>B</strong> representing the borders of the range <strong>[A, B]</strong> in which we want to count stapled intervals (<strong>1&nbsp;</strong><span style="font-weight: bold;">��</span><strong>&nbsp;A&nbsp;</strong><span style="font-weight: bold;">��</span><strong>&nbsp;B&nbsp;</strong><span style="font-weight: bold;">��</span><strong>&nbsp;10<sup>7</sup></strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print <strong>P</strong> lines, each with a single integer number. For <strong>i = 1, 2, ..., P</strong> the number in the <strong>i</strong>-th line represents the number of stapled intervals completely contained in the range <strong>[A, B]</strong> corresponding to the <strong>i</strong>-th question.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
2184 2200
2185 2200
2184 2199
1 100000</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1
0
0
13</span><span style="white-space: normal;">
</span></pre>