<p>
Jimmy is a hard-working pupil in his second year at primary 
school. Recently he decided to convert all his notes into an
electronic version. Sadly, he found that 
his math notes were full of ink blots.
</p>

<p>
He scanned the notes and sent them through his own OCR package
(yes, he coded it all by himself at the age of 8).
The OCR package replaced all ink blots by the string "<code>machula</code>".
</p>

<h3>Problem specification</h3>

<p>
You are given Jimmy's notes, processed by the OCR. They contain simple 
math exercises, which were used to practice addition on positive integers. 
Your task is to recover the damaged part of the notes.
</p>

<h3>Input specification</h3>

<p>
The first line of the input file contains an integer <b>T</b> specifying the
number of test cases. Each test case is preceded by a blank line.
</p>

<p>
Each test case consists of exactly one line. 
The line represents an equation of the form "<code>number + number = number</code>",
where each <code>number</code> is a positive integer. 
One part of the equation will be replaced by the string "<code>machula</code>".
The string always covers a contiguous non-empty sequence of digits, possibly even an entire
number. You may assume that for each equation in the input there will be 
exactly one way to fill in the missing digits.
</p>

<h3>Output specification</h3>

<p>
For each test case, the output shall contain one line of the form 
"<code>number + number = number</code>". The line must represent the equation
from that test case with all missing digits filled in.
</p>

<h3>Example</h3>

<b>Input:</b><br>
<pre>3

23 + 47 = machula

3247 + 5machula2 = 3749

machula13 + 75425 = 77038
</pre>

<b>Output:</b><br>
<pre>23 + 47 = 70
3247 + 502 = 3749
1613 + 75425 = 77038
</pre>
<p>Note: <b>int</b> in C++/C/Java or <b>longint</b> in Pascal is enough.</p>