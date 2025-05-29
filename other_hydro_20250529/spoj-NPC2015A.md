<p>Eefun is currently learning to read. His way of learning &nbsp;is unique, by trying to make every possible substring from a given string. However, when the string becomes longer, he can no longer remember all the substring. His friends want to test Eefun's skill by asking questions, given a string S, is there any substring that begins with letter X and ends with letter Y? According to Eefun, each substring contains at least 2 letters. As the given string S is pretty big, Eefun need your help to answer his friend's questions</p>
<h3>Input</h3>
<p>First line of input contain a single string S which was given by his friends.<br>Second line contain a number N, the number of questions that Eefun's friends ask.<br>Next N lines each consists of 2 characters, X and Y</p>
<h3>Output</h3>
<p>For each questions, output a single string "YA" if the substring exists, or "TIDAK" otherwise<br>(YA means yes and TIDAK means no in Indonesian)&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
HALO<br>4<br>H O<br>L O<br>A O<br>O L&nbsp;</pre>
<pre><strong>Output:</strong>
YA<br>YA<br>YA<br>TIDAK&nbsp;</pre>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraints:</h3>
<ul>
<li>'A' ¡Ü X,Y ¡Ü 'Z'</li>
<li>1 ¡Ü |S| ¡Ü 1.000.000</li>
<li>1 ¡Ü N ¡Ü 1.000.000</li>
</ul>
</div>