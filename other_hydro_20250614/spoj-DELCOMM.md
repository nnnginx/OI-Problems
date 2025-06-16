<p>It is required to find out whether it is possible to delete given files
from MS-DOS directory
executing the DEL command of MS-DOS operation system only once.
There are no nested subdirectories.</p>
<h3>A note</h3>
<p>
DEL command has the following format: <tt>DEL</tt> <em>wildcard</em>

</p><p>

</p><p>
<br>
The actual wildcard as well as a full file name can be made up either of
a name containing 1 up to 8
characters or of a name and extension, containing up to 3 characters.
The point character '.' separates the extension from the file name.
The extension can be empty and this is equivalent to a
name without any extension (in this case a wildcard ends with a point).
In a wildcard the characters
'?' and '*' can be used. A question mark substitutes exactly one character
of the full file name
excluding a point, an asterisk any sequence of characters
(containing no points) even empty one.
An asterisk can appear only at the last position of the name and the extension.

</p><p>

</p><p>
<br>
MS-DOS system can permit maybe other wildcards but they can not be used
in this task. File names
and extensions consist only of Latin capitals and digits.

</p><p>
</p><h3>Input</h3>
<p>The first line of the input is an integer M, then a blank line followed by M datasets. There is a blank line between datasets.

</p><p>Input data for each dataset contains a list of full file names without empty lines
and spaces. Each
name is written in a separate line of input data file and preceded with
a control sign: '-' for delete
or '+' for keep. Full file names are not repeated. The list comprises
at least one file, and at least one
file is marked to be deleted. There are no more than 1000 files.

</p><p>
</p><h3>Output</h3>
<p>
For each dataset, write to the first line of output the required DEL command
(only one
proposal) or <tt>IMPOSSIBLE</tt> if there is no solution.
A space should separate "<tt>DEL</tt>" from wildcard.
<b>Print a blank line between datasets.</b>

</p><p>
</p><h3>Example</h3>

<pre><b>Input:</b>

1

-BP.EXE
-BPC.EXE
+TURBO.EXE

<b>Output:</b>

DEL ?P*.*
</pre>