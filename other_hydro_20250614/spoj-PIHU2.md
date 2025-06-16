<p>Last time you helped Rancho getting kisses from Pihu. This time Pihu needs your help in determining the number of, different ways of kissing.</p>
<p>Actually the story goes this way.</p>
<p>Rancho will fix a certain number of days, say <strong>N</strong> (<strong>N &lt;= 10^18</strong>). Now Pihu as usual, will kiss Rancho each day, but this time there will be rules for kissing. Rules go below:-</p>
<p>Suppose for a certain number of days <strong>N</strong>, Pihu needs to learn <strong>P</strong>&nbsp;different ways of kissing. She can kiss Rancho on every day with any number of kisses (of-course less than or equal <strong>P</strong>), but all the kisses should be different from each other. Also to keep ※Kissing of each day§ unique, between every pair of days ,say day <strong>i</strong> and day<strong> j</strong> (<strong>i</strong> not equal <strong>j</strong>) , day<strong> i</strong> must have at-least one type of kiss that day <strong>j</strong> does not have and day <strong>j</strong> must have at-least one type of kiss that day <strong>i</strong> does not have. (Refer explanation below)</p>
<p>Help Pihu, determine the minimum number of different ways/types of kissing for <strong>N</strong> days 每 call the minimum number as <strong>P</strong>.</p>
<p><strong>Explanation:</strong></p>
<p>Suppose on day <strong>i</strong>, Pihu kisses Rancho with a set <strong>S<sub>i</sub></strong>&nbsp;每 (k<sub>1</sub>, k<sub>2</sub>, k<sub>3</sub>, ＃＃.. k<sub>m &nbsp;</sub>: k<sub>1</sub>≧k<sub>2</sub>≧k<sub>3</sub>≧＃＃≧k<sub>m</sub>) kisses and on day<strong> j</strong> with a set <strong>S<sub>j</sub></strong>&nbsp;每 (k<sub>1</sub>, k<sub>2</sub>, k<sub>3</sub>, ＃＃＃. k<sub>l</sub>&nbsp;: k<sub>1</sub>≧k<sub>2</sub>≧k<sub>3</sub>≧＃＃≧k<sub>l</sub>), then there should be at-least one k<sub>i</sub> in set <strong>S<sub>i</sub></strong>&nbsp;that is not in set <strong>S<sub>j</sub></strong>&nbsp;and there should be at-least one k<sub>j</sub> in set <strong>S<sub>j</sub></strong>&nbsp;that is not in set <strong>S<sub>i</sub></strong>. Thus you can consider <strong>P </strong>as the size of the superset of S<sub>1</sub> ,S<sub>2</sub> ,S<sub>3</sub> ,........ S<sub>N</sub> .</p>
<h3>Input</h3>
<p>The first line of input consists of the number of test cases <strong>T (T &lt;= 100000)</strong>.</p>
<p>Next follows <strong>T</strong> lines, with each line consisting of one number <strong>N</strong> 每 the number of days &nbsp;<strong>(1 &lt;= N &lt;= 10^18)</strong>.&nbsp;</p>
<h3>Output</h3>
<p>For each test case print the minimum number of different ways of kissing 每<strong>&nbsp;P</strong>&nbsp;on separate lines.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3</pre>
<pre>1</pre>
<pre>2</pre>
<pre>3</pre>
<pre><strong>Output:</strong></pre>
<pre>1</pre>
<pre>2</pre>
<pre>3
</pre>