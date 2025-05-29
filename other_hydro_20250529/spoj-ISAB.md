<p>Isabella and Steve are very good friends, and they often write letters to each other. They exchange funny experiences, talk about people around, share their feelings and write about almost everything through the letters. When the letters are delivered, they are quite afraid that some other people(maybe their parents) would peek. So they encrypted the letter, and only they know how to decrypt it. This guarantees their privacy.</p>

<p>The encrypted message is an <b>N</b>��<b>N</b> matrix, and each grid contains a character.</p>

<p>Steve uses a special mask to work as a key. The mask is <b>N</b>��<b>N</b>(where <b>N</b> is an even number) matrix with (<b>N</b>��<b>N</b>)/4 holes of size <b>1</b>��<b>1</b> on it.</p>

<p>The decrypt process consist of the following steps:</p>

<ol>
<li>Put the mask on the encrypted message matrix.</li>
<li>Write down the characters you can see through the holes, from top to down, then from left to right.</li>
<li>Rotate the mask by 90 degrees clockwise.</li>
<li>Go to step 2, unless you have wrote down all the <b>N</b>��<b>N</b> characters in the message matrix.</li>
<li>Erase all the redundant white spaces in the message.</li>
</ol>

<p>For example, you got a message shown in figure 1, and you have a mask looks like figure 2. The decryption process is shown in figure 3, and finally you may get a message <tt>"good morning"</tt>.</p>

<img src="/content/crazyb0y:ISAB12.png">

<img src="/content/crazyb0y:ISAB3.png">

<p>You can assume that the mask is always carefully chosen that each character in the encrypted message will appear exactly once during decryption.</p>

<p>However, in the first step of decryption, there are several ways to put the mask on the message matrix, because the mask can be rotated (but not flipped). So you may get different results such as <tt>"od morning go"</tt> (as showed in figure 4), and you may also get other messages like <tt>"orning good m"</tt>, <tt>"ng good morni"</tt>.</p>

<img src="/content/crazyb0y:ISAB4.png">

<p>Steve didn't know which direction of the mask should be chosen at the beginning, but after he tried all possibilities, he found that the message <tt>"good morning"</tt> is the only one he wanted because he couldn't recognize some words in the other messages. So he will always consider the message he can understand the correct one. Whether he can understand a message depends whether he knows all the words in the message. If there are more than one ways to decrypt the message into an understandable one, he will choose the lexicographically smallest one. The way to compare two messages is to compare the words of two messages one by one, and the first pair of different words in the two messages will determine the lexicographic order of them.</p>

<p>Isabella sends letters to Steve almost every day. As decrypting Isabella's message takes a lot of time, and Steve can wait no longer to know the content of the message, he asked you for help. Now you are given the message he received, the mask, and the list of words he already knew, can you write a program to help him decrypt it?</p>


<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 �� <b>T</b> �� 100), indicating the number of test cases.</p>

<p>Each test case contains several lines. The first line contains an even integer <b>N</b> (2 �� <b>N</b> �� 50), indicating the size of the matrix.</p>

<p>The following <b>N</b> lines each contains exactly <b>N</b> characters, reresenting the message matrix. The message only contains lowercase letters and periods(<tt>'.'</tt>), where periods represent the white spaces. You can assume the matrix contains at least one letter.</p>

<p>The following <b>N</b> lines each contains <b>N</b> characters, representing the mask matrix. The asterisk(<tt>'*'</tt>) represents a hole, and period(<tt>'.'</tt>) otherwise.
The next line contains an integer <b>M</b>(1 �� <b>M</b> �� 100), the number of words he knew.</p>

<p>Then the following <b>M</b> lines each contains a string represents a word. The words only contain lowercase letters, and its length will not exceed 20.</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is Isabella's message.</p>
<p>If Steve cannot understand the message, just print the <b>Y</b> as <tt>"FAIL TO DECRYPT"</tt>.</p>



<h3>Example</h3>

<pre><b>Input:</b>
3
4
o.do
.ng.
grmn
o.i.
.*..
*.*.
....
*...
2
good
morning
4
..lf
eoyv
oeou
vrer
..*.
.*..
....
*.*.
5
i
you
the
love
forever
4
.sle
s.c.
e.fs
..uu
*...
.*..
...*
..*.
1
successful

<b>Output:</b>
Case #1: good morning
Case #2: love you forever
Case #3: FAIL TO DECRYPT
</pre>