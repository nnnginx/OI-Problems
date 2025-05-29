<p> In a rectangular field of size n by m squares there is a mouse and two cats. The mouse is the first to make a move, then each of the cats makes a move, then again its the mouse's turn, and so on. In each move both the mouse and the cats can move exactly one square vertically or horizontally. If the mouse is standing at the edge of the field then in its next move it can jump off the field and is saved from the cats. If in the next move one of the cats moves to the field with the mouse then there is no escape for the mouse ... =(<br><br>
You are to write a program which, knowing the initial positions of mouse and the two cats, will find out if there is any way for the mouse to escape from the cats, assuming of course that each cat will do its best to catch the mouse.<br>

</p><h3>Input</h3>
<p>In the first line of input two integers n and m are given, not exceeding 100, where n is the number of rows, and m - the number of columns. The second line contains a number k [k &lt;= 10], which defines the number of test cases for the given field. In the next k lines the initial positions of the mouse and the cats are given. The position in the field is given by two numbers: the first is the number of the row, the second is the number of the column. The first two integers are the coordinates of the mouse, the next four integers are the coordinates of the cats.</p>
 
<h3>Output</h3>
<p> You must output k lines with answers for each test case. The answer is YES, if the mouse can escape or NO otherwise.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5 3
3
2 2 1 1 3 3
2 3 1 3 5 2
3 2 1 2 4 3

<b>Output:</b>
NO
YES
YES
</pre>

<h3>Author: Filimonenkov D.O.</h3>