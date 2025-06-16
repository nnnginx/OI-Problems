<p>
One of your friends wants to write his own archiver. He is going to replace neighboring equal substrings with only one copy. For example, he is going to change substring "AA" with something like "2(A)" and if "A" is long enough it will reduce the file size.
<br><br>
But, before performing any coding stuff he wants to know how many such double substrings are there in the input file.
<br><br>
He asks you to help him, because this task is very difficult for him.

</p><h3>Input</h3>
<p>Input file contains the text to be archived. It will only contain Latin letters (big and small). Its size will not exceed 200000 symbols. Letters are case sensitive, i.e. "X" is not equal to "x".

</p><h3>Output</h3>
<p>Write a number of substrings of input text which can be written as "AA", i.e. consist of two equal concatenated parts.

</p><h3>Example</h3>

<pre><b>Input:</b>
abcdefg

<b>Output:</b>
0
</pre>

<pre><b>Input:</b>
blabla

<b>Output:</b>
1
</pre>

<pre><b>Input:</b>
aCacaacaa

<b>Output:</b>
4
</pre>