<p align="justify">
You are given a text. Calculate the minimum number of keystrokes needed
to produce this text,
if the editor described below is used.
<br>
If you haven't read the problem "Editor" before, here is a description
of the functionality of the editor:
</p>
<div align="left">
<ul>
<li>'\n': begin a new line. If the last line was empty, stop
processing and print out all lines.</li>
<li>'d': copy all characters from the current line, and append them
after
the last character in this line. For example, if current line contains
ab, and d is pressed two times, the result will be abababab</li>
<li>any other character: append it to the current line.</li>
</ul>
</div>
<h3>Input</h3>
<p align="justify">
The input consists of <b>exactly ten</b> test cases.
Each test case consists of a line with at most 600 characters. The
character 'd' is not used in any of the lines, but all other printable ascii characters may occur.
</p>
<h3>Output</h3>
<p align="justify">
For each test case, first print a line containing the minimum number of
key strokes to produce the given line of text.
In the next lines, write the keys that are pressed to produce the text.
If there are several possibilites with minimum number of keystrokes,
you should also minimise the number of lines,
if there is still more than one possibility, minimise number of
keystrokes before the first '\n', then second '\n', ...
</p><p>
Since 'd' is a costly operation in the editor, for each output line you
should minimise the number of 'd' characters as the 2nd criterion after
minimising number of keystrokes in this line.
</p><p>
The original input line should be the same as the output of the editor (processing the output you produce), if '\n' characters are ignored.
</p><p>
<b>Notice that you have to terminate the input for the editor with two
'\n'.</b>
</p>
<h3>Example</h3>
<p>Here only two test cases.</p>
<pre><b>Input:</b>

00001123444456789<br>000011234444446789

<b>Output:</b>
18
00d1123444456789

18
00d1123
444d6789


</pre>