<p>
Bruce Force's keyboard is broken, only a few keys are still working. Bruce has
figured out he can still type texts by switching the keyboard layout whenever
he needs to type a letter which is currently not mapped to any of the <i>m</i>
working keys of the keyboard.
</p>
<p>
You are given a text that Bruce wishes to type, and he asks you if you can tell him
the maximum number of consecutive characters in the text which can be typed without
having to switch the keyboard layout.
For simplicity, we assume that each key of the keyboard will be mapped to exactly one character, and it is not possible to type other characters by combination of different keys.
This means that Bruce wants to know the length of the largest substring of the text
which consists of at most <i>m</i> different characters.
</p>
<h3>Input</h3>
<p>The input contains several test cases, each test case consisting of two lines.
The first line of each test case contains the number <i>m</i> (<i>1 ¡Ü m ¡Ü 128</i>),
which specifies how many keys on the keyboard are still working.
The second line of each test case contains the text which Bruce wants to type.
You may assume that the length of this text does not exceed 1 million characters.
Note that the input may contain space characters, which should be handled like any other character.
</p>
<p>
The last test case is followed by a line containing one zero.
</p>
<h3>Output</h3>
<p>For each test case, print one line with the length of the largest substring
of the text which consists of at most <i>m</i> different characters.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
5
This can't be solved by brute force.
1
Mississippi
0

<b>Output:</b>
7
2
</pre>