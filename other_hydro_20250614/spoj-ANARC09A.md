<p>I¡¯m out of stories. For years I¡¯ve been writing stories, some rather silly, just to make simple problems look difficult and complex problems look easy. But, alas, not for this one.</p>
<p>You¡¯re given a non empty string made in its entirety from opening and closing braces. Your task is to find the minimum number of ¡°operations¡± needed to make the string stable. The definition for being stable is as follows:</p>
<ol>
<li>An empty string is stable.</li>
<li>If S is stable, then {S} is also stable.</li>
<li>If S and T are both stable, then ST (the concatenation of the two) is also stable.</li>
</ol>
<p>All of these strings are stable: {}, {}{}, and {{}{}}; But none of these: }{, {{}{, nor {}{. <br>The only operation allowed on the string is to replace an opening brace with a closing brace, or visa-versa.</p>
<h3>Input</h3>
<p>Your program will be tested on one or more data sets. Each data set is described on a single line. The line is a non-empty string of opening and closing braces and nothing else. No string has more than 2000 braces. All sequences are of even length.</p>
<p>The last line of the input is made of one or more ¡¯-¡¯ (minus signs.)</p>
<h3>Output</h3>
<p>For each test case, print the following line:</p>
<p>k. N</p>
<p>Where k is the test case number (starting at one,) and N is the minimum number of operations needed to convert the given string into a balanced one.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
}{<br>{}{}{}<br>{{{}<br>---<br><br><strong>Output:</strong>
1. 2<br>2. 0<br>3. 1</pre>