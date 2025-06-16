<p>A team of speleologists organizes a training in the Great Cave of&nbsp;Byte Mountains.
During the training each speleologist explores a route from Top Chamber
to Bottom Chamber. The speleologists may move down only, i.e. the level of every
consecutive chamber on a route should be lower then the previous one. Moreover, each
speleologist has to start from Top Chamber through a different corridor and each of them must enter
Bottom Chamber using different corridor. The remaining corridors may be traversed by
more than one speleologist. How many speleologists can train
simultaneously?&nbsp;
</p>


<h3>Task</h3>

<p>
Write a program which:
</p><ul>  
 	<li>reads the cave description from the standard input,
 	</li><li>computes the maximal number of speleologists that may train
      simultaneously,
 	</li><li>writes the result to the standard output.
</li></ul>  

<h3>Input</h3>
<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
In the first line of each test case there is one integer <i>n</i>
(<i>2&lt;=n&lt;=200</i>), equal to the number of chambers in the cave. The chambers are
numbered with integers from <i> 1</i> to <i> n</i> in descending level order - the chamber of
grater number is at the higher level than the chamber of the lower one. (Top
Chamber has
number <i>1,</i> and Bottom Chamber has number <i>n</i>). In the following <i>n-1</i>lines
(i.e. lines <i>2,3,...,n</i>) the descriptions of corridors are given. The (<i>i+1</i>)-th
line contains numbers of chambers connected by corridors with the <i>i</i>-th chamber. (only
chambers with numbers grater then <i>i</i> are mentioned). The first number in a line, <i>m</i>, <i>
0&lt;=m&lt;=</i>(<i>n-i+1</i>), is a number of corridors exiting the chamber being described.
Then the following<i> m</i> integers are the numbers of
the chambers the corridors are leading to.&nbsp;
</p>

<h3>Output</h3>

<p>
Your program should write one integer for each test case.
This number should be equal to the maximal number of
speleologists able to train simultaneously,
</p>

<h3>Example</h3>

<pre><b>Sample input:</b>
1
12
4 3 4 2 5
1 8
2 9 7
2 6 11
1 8
2 9 10
2 10 11
1 12
2 10 12
1 12
1 12

<b>Sample output:</b>
3
</pre>

<p>The sample input corresponds to the following cave:<br>
<img src="/content/piotrek:grotol.gif" height="426" width="249"> 
</p>