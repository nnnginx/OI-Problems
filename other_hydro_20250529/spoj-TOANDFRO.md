<p>Mo and Larry have devised a way of encrypting messages. They first decide secretly on the number of
columns and write the message (letters only) down the columns, padding with extra random letters so
as to make a rectangular array of letters. For example, if the message is ��There��s no place like home on
a snowy night�� and there are five columns, Mo would write down
</p>
<p></p><pre>t o i o y
h p k n n
e l e a i
r a h s g
e c o n h
s e m o t
n l e w x
</pre>
<p></p>
<p>Note that Mo includes only letters and writes them all in lower case. In this example, Mo used the
character ��x�� to pad the message out to make a rectangle, although he could have used any letter.
Mo then sends the message to Larry by writing the letters in each row, alternating left-to-right and
right-to-left. So, the above would be encrypted as
</p>
<p></p><pre>toioynnkpheleaigshareconhtomesnlewx</pre>
<p></p>
<p>Your job is to recover for Larry the original message (along with any extra padding letters) from the
encrypted one.</p>
<h3>Input</h3>
<p>There will be multiple input sets. Input for each set will consist of two lines. The first line will contain
an integer in the range 2...20 indicating the number of columns used. The next line is a string of up
to 200 lower case letters. The last input set is followed by a line containing a single 0, indicating end of
input.</p>
<h3>Output</h3>
<p>Each input set should generate one line of output, giving the original plaintext message, with no spaces.</p>
<h3>Example</h3>

<pre><b>Input:</b>

5
toioynnkpheleaigshareconhtomesnlewx
3
ttyohhieneesiaabss
0

<b>Output:</b>

theresnoplacelikehomeonasnowynightx
thisistheeasyoneab
</pre>