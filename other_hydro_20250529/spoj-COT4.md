<p>Maintain two sets of strings <b>S</b> and <b>T</b>. Initially, each set contains an empty string with id 1.</p>
<p>
Your program are to perform the following four operations:
</p>
<ol>
  <li>Add a char <b>c</b> to the end of an existed string <b>Si</b> in <b>S</b>, then insert the new string into <b>S</b>. Since there has been <b>n</b> strings in <b>S</b> already, the new string will hold the id <b>n+1</b>.</li>
  <li>Add a char <b>c</b> to the beginning or to the end of an existed string <b>Ti</b> in <b>T</b>, then insert the new string into <b>T</b>.</li>
  <li>Choose two existed strings <b>Ti</b> and <b>Tj</b> from <b>T</b>, next combine them into a new one <b>TiTj</b>, then insert the new string into <b>T</b>.</li>
  <li>Print the time that an existed string <b>Ti</b> in <b>T</b> appears in an string <b>Si</b> in <b>S</b>. Your program should print <tt>0</tt> if <b>Ti</b> is an empty string.</li>
</ol>

<h3>Input</h3>
<p>In the first line, there is an integer <b>Q</b>, which means the number of operations to perform.</p>
<p>In the next <b>Q</b> lines,the <b>i</b>-th line describes the <b>i</b>-th operation containing some integers. Such a line may look like this:</p><p>
</p><ul>
  <li><tt>1 Si c</tt></li>
  <li><tt>2 0 Ti c</tt> =&gt; add <b>c</b> to the beginning of <b>Ti</b></li>
  <li><tt>2 1 Ti c</tt> =&gt; add <b>c</b> to the end of <b>Ti</b></li>
  <li><tt>3 Ti Tj</tt></li>
  <li><tt>4 Ti Si</tt></li>
</ul>
<p><b>Q</b> &lt;= 300000, 'a' &lt;= <b>c</b> &lt;= 'z'</p>

<p>The number of the first operation will not exceed 100000.&nbsp;</p>
<p>The number of the third operation will not exceed 30000.</p>
<p>The number of fourth operation will not exceed 100000.</p>

<h3>Output</h3>
<p>For each <tt>"4 Ti Si"</tt> operation, print its result.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
18
1 1 a
1 2 a
1 3 b
1 2 b
1 5 a
1 5 b
2 1 1 a
3 2 2
2 0 3 b
2 1 2 b
3 2 5
3 5 2
4 7 6
4 5 6
4 3 4
4 2 4
4 2 7
4 2 6

<strong>Output:</strong>
1
1
1
2
1
2</pre>