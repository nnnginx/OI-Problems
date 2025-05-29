<p align="justify">
Have you ever programmed in Brainf**k? If yes, then you know how
annoying it is to press the same key several times in a row. So what we all
need, is a good editor.
Here are the functions that the editor should have:
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
<p align="justify">
<b>Please note, that the solution may only be submitted in Brainf**k or
Intercal.</b>
</p>
<h3>Input</h3>
<p align="justify">
There is exactly one test case. You can assume, that there is no key press of 'd' when the line is still empty.
</p>
<h3>Output</h3>
<p align="justify">
Print the output that the editor described above would produce on the given input. You can assume, that no line is created with more than 150 characters.
</p>
<h3>Example</h3>
<p>
</p><pre><b>Input:</b>

sample-test<br>-dd-d-dd<br>end signalled by two newlines<br><br>

 
<b>Output:</b>

sample-test<br>--------------------------------------------<br>enen signalleenen signalle by two newlines<br></pre><p></p>