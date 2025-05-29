<p>Have you ever used a text editor like notepad ++ or sublime? In the text editor software, several lines can be selected at once so that in 1x the tab key on the keyboard is pressed, all lines will move forward. Or press Shift Tab 1x then all the selected lines will be backward together. Selection of rows must be carried out sequentially (for example selecting rows 1 to line 5) and should not select lines that are jumped (not consecutive).</p>
<h3>Input</h3>
<p>Input begins with a T representing a testcase (1 &lt;= T &lt;= 100) and is followed by N (amount of text, 1&lt;=N&lt;=100000) inside the text editor. Each text in the text editor has an initial tab position. The line after N is the starting tab position of each text. Two Lines after N is the tab position the goal is to reach.</p>
<h3>Output</h3>
<p>Each time the Tab key or Shift Tab key is pressed will count as one press of the key. Find the minimum number of Tab or Shift Tab presses to reach the destination.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>3</pre>
<pre>1 2 3<br>3 4 5

<strong>Output:</strong>
2
</pre>