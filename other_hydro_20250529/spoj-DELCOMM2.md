<p>It is required to find out what's the maximum number of files that can be deleted from MS-DOS directory
executing the DEL command of MS-DOS operation system only once.
There are no nested subdirectories.</p>
<h3>A note</h3>
<p>
DEL command has the following format: <tt>DEL</tt> <em>wildcard</em>

</p><p>

</p><p>
<br>
The actual wildcard as well as a full file name can be made up of
a name containing 1 up to 8 case-sensitive characters.
In a wildcard the characters
'?' and '*' can be used. A question mark substitutes exactly one character
of the full file name, an asterisk any sequence of characters even empty one.
</p><p>

</p><p>
<br>
MS-DOS system can permit maybe other wildcards but they can not be used
in this task. File names
consist only of Latin letters and digits.

</p><p>
</p><h3>Input</h3>
<p>The first line of the input is an integer M, then a blank line followed by M datasets. There is a blank line between datasets.

</p><p>Input data for each dataset contains a list of full file names without any extra empty lines
and spaces. Each
name is written in a separate line of input data file and ended with
a control sign: '+' for delete
or '-' for keep. Full file names are not repeated. The list comprises
at least one file, and at least one
file is marked to be deleted. There are no more than 250 files.

</p><p>
</p><h3>Output</h3>
<p>
For each dataset, write to the first line of output the maximum number of files one DEL command can delete.

</p><p>
</p><h3>Example</h3>

<pre><b>Input:</b>

2

BP +
BPC +
TURBO -

EXCHANGE +
EXT +
HARDWARE +
MOUSE ¨C
NETWORK ¨C

<b>Output:</b>

2
2
</pre>
<b>Hint:</b>
<p>For the two tests above,the corresponding DEL commands are DEL BP* and DEL EX*.</p>
<h3>Link</h3>
<p>You can try problem <a href="http://www.spoj.com/problems/DELCOMM">DELCOMM</a> first. It's far easier than this problem.</p>