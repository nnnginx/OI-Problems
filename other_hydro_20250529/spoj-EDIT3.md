<h3>Background</h3>
<p>After trying to solve problem EDIT1(Editor) and being ****ed by Brainf**k, Blue Mary decided to set another difficult problem about editor.</p>
<h3>Description</h3>
<p>Some definations:</p>
<div>
<ul>
<li> Text: It's a sequence that consists characters whose ASCII code is in [32,126]. </li>
<li> Cursor: It's a sign for pointing out the current position.It can be at the start or the end of the text or between two consecutive characters of the text.</li>
</ul>
</div>
<p>Editor is a structure.It contains one text and one cursor.The operations are listed below:</p>
<pre>--------------------------------------------------------------------------
| Name        | Input format |              function                     |
--------------------------------------------------------------------------
| Move(k)     | Move k       | Move the cursor after the kth character   |
|             |              | in the text. If k=0, you should put       |
|             |              | the cursor at the start of the text.      |
--------------------------------------------------------------------------
| Insert(n,s) | Insert n s   | Insert string s whose length is n(&gt;=1)    |
|             |              | after the cursor.The cursor doesn't move. |
--------------------------------------------------------------------------
| Delete(n)   | Delete n     | Delete n(&gt;=1) characters after the cursor.|
|             |              | The cursor doesn't move.                  |
--------------------------------------------------------------------------
| Get(n)      | Get n        | Output n(&gt;=1) characters after the cursor.|
--------------------------------------------------------------------------
| Prev()      | Prev         |  Move the cursor one character forward.   |
--------------------------------------------------------------------------
| Next()      | Next         |  Move the cursor one character backward.  |
--------------------------------------------------------------------------
</pre>
<p>If the text of a editor is empty,we say the editor is empty.</p>
<p>Here is an example._ denotes to the cursor,$ denotes to the start and the end.At start the editor is empty.</p>
<pre>------------------------------------------------------------------------------
|         Operation          |  Text after the operation |        Output     |
------------------------------------------------------------------------------
| INSERT(13,"Balanced tree") |  $_Balanced tree$         | $$                |
------------------------------------------------------------------------------
| MOVE(2)                    |  $Ba_lanced tree$         | $$                |
------------------------------------------------------------------------------
| DELETE(5)                  |  $Ba_d tree$              | $$                |
------------------------------------------------------------------------------
| NEXT()                     |  $Bad_ tree$              | $$                |
------------------------------------------------------------------------------
| INSERT(7," editor")        |  $Bad_ editor tree$       | $$                |
------------------------------------------------------------------------------
| MOVE(0)                    |  $_Bad editor tree$       | $$                |
------------------------------------------------------------------------------
| GET(15)                    |  $_Bad editor tree$       | $Bad editor tree$ |
------------------------------------------------------------------------------
</pre>
<p>Your task is:</p>
<div>
<ul>
<li> Build an empty editor. </li>
<li> Read some operations from the standard input and operate them. </li>
<li> For each Get operation, write the answer to the output.</li>
</ul>
</div>
<h3>Input</h3>
<p>the very first line contains the number of testcases T(T&lt;=4).T tests follow.</p>
<p>For each test, the first line is the number of operations N.N operations follow.</p>
<p>Blue Mary is so depressed with the problem EDIT1 that she decides to make the problem  more difficult.So she inserts many extra line breaks in the string of the Insert operation.You must ignore them.</p>
<p>Except line breaks, all the charaters' ASCII code are in [32,126]. There's no extra space at the end of a line.</p>
<p>You can assume that for each test case:</p>
<div>
<ul>
<li> No invalid operation is in the input. </li>
<li> Number of move operations is no more than 50000. </li>
<li> Number of the total of insert and delete operations is no more than 4000. </li>
<li> Number of the total of prev and next operations is no more than 200000. </li>
<li> The characters inserted will not more than 2MB.The valid output will not more than 3MB. </li>
</ul>
</div>
<h3>Output</h3>
<p>The output should contain T blocks corresponding to each testcase.</p>
<p>For each test case, the output should contain as many lines as the get operations in the input.Each line should contains the output of each get operation.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
15
Insert 26
abcdefghijklmnop
qrstuv wxy
Move 15
Delete 11
Move 5
Insert 1
^
Next
Insert 1
_
Next
Next
Insert 4
.\/.
Get 4
Prev
Insert 1
^
Move 0
Get 22

<strong>Output:</strong>
.\/.
abcde^_^f.\/.ghijklmno
</pre>
<p><strong>Warning: large Input/Output data, be careful with certain languages</strong></p>