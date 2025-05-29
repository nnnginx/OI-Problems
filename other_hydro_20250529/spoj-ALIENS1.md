<p>Little Johnny of Byteland has been kidnapped by aliens from the Andromeda galaxy! Johnny is currently locked in a small room inside an UFO, which has been parked in his backyard. Johnny is desparately trying to open the door of the room. He finds that the door asks a series of arithmetic questions: addition, subtraction, mutltiplication or exponentiation (the aliens dont know how to divide) of two given numbers. Johnny laughs aloud and thinks that it will be very easy to answer these questions and escape. But when he sees the questions, he realises that the aliens use base 42! Now Johnny has panicked and asks you to help him out.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p><br>The first line of the input has a number T (&lt;= 500), denoting the number of tests cases. T lines follows, each of the form A op B, where A and B are numbers in base 42 having upto 10000 digits without unnecessary zeros and op is either +, -, * or ^ denoting the operation to be performed. Base 42 numbers are denoted by:</p>
<p>'0' to '9' denotes 0 to 9</p>
<p>'A' to 'Z' denotes 10 to 35</p>
<p>'a' to 'f' denotes 36 to 41</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case, output one line: the result of the required&nbsp;operation in base 42 modulo LIFE<sub>42</sub>, without any unnessary zeros.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
11
a + a
e - A
91 * 89
AEIOU + abcd
A - B
b ^ 2
5 ^ 0
123 - 45
ABC * 10
6 - 6
0 ^ 0

<strong>Output:</strong>
1U
U
1W59
L6ZR
LIFD
WP
1
de
ABC0
0
1</pre>
<pre><strong><span style="font-size: large;">Warning: large Input/Output data, be careful with certain languages.</span></strong></pre>