<p>Shmoogle company developed new protocol &lt;&lt;Wave&gt;&gt; for the multi-user online editing of the text data. Using it, any client can send commands to the server for editing the text and the server would broadcast it to all other connected clients. Each command consists of a sequence of operations of the following type:
</p><blockquote class="table"><div class="center"><div class="center"></div>
<table border="1" cellpadding="1" cellspacing="0"><tbody><tr><td align="center" nowrap="nowrap" valign="top"> Operation</td><td align="left" valign="top">Description</td></tr>
<tr><td align="center" nowrap="nowrap" valign="top"> <tt>R</tt> <i>k</i></td><td align="left" valign="top">Moves the cursor <i>k</i> positions right. The cursor is positioned at before the first character of the text at the start of performing the command.</td></tr>
<tr><td align="center" nowrap="nowrap" valign="top"> <tt>C</tt> <i>k</i> <i>s</i></td><td align="left" valign="top">Inserts the string <i>s</i> of length <i>k</i> at the cursor position. After this operation the cursor is positioned to the right of the inserted string.</td></tr>
<tr><td align="center" nowrap="nowrap" valign="top"> <tt>D</tt> <i>k</i></td><td align="left" valign="top">Deletes <i>k</i> characters right of the cursor.</td></tr>
</tbody></table>
<div class="center"></div></div></blockquote><p>When the new client connects the server needs to send it all the command this client missed. In order to save traffic the server merges all the commands in one equivalent command. Help Shmoogle company implement merging of commands effectively.</p><p>The resulting command should consist of the least possible number of operations. The delete operations should precede the insert operations if possible.</p>

<h3>Input</h3>
<p>The first line contains T (1 &lt;= T &lt;= 10) ¡ª the number of test cases. The description of T tests follow.

The first line of each test case contains the amount of commands n (1 &lt;= n &lt;= 10000). The description of each command follows. The first line of each command contains the amount of operations m (1 &lt;= m &lt;= 10). The next m lines contain the description of each operation in the format given above. 1 &lt;= k &lt;= 100000 for R and D operations, and 1 &lt;= k &lt;= 10 for C operations. The strings in C operations consist of latin letters and digits only.

</p><h3>Output</h3>
<p>For each test case your program should print the result of merging the commands. The format of the command should be the same as in the input file, except for the limitations on m and k. The result should consist of the least possible number of operations. The delete operations should precede the insert operations if possible. If the result of merging consist of no operations print 0.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2
4
R 4
C 3 abc
R 2
C 3 xyz
3
R 7
C 3 def
D 3

<b>Output:</b>
3
R 4
D 2
C 8 abcdefyz

</pre>