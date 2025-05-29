<p>You won the lottery tickets to visit the famous Disneyland HongKong with the Taarak Mehta ka Ulta Chasma family and Subramaniam Iyer gets stuck in the Honey Comb maze. He has a Phone along with him and no one else to help him out. He calls you and asks for help. Chuck the story getting into the problem now , There are N x M blocks of Honey combs in the maze and you are given a starting point. your task is to help Mr. Iyer find out whether or not he can traverse the maze and return to his original position. The constraint being that a honey comb ( Block ) once visited cannot be visited again . Also , he has to make a minimum of 'k' number of moves before returning to the starting point . &nbsp;The '.' represent the emty blocks whereas the '*' represent the blocks that can't be visited . from a block (x,y) Iyer can move only to blocks (x-1,y) &nbsp;, &nbsp;(x+1,y) &nbsp;, &nbsp;(x,y+1) &nbsp;, &nbsp;(x,y-1) . Help Mr. Iyer return to his original position.&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input contains the dimensions &nbsp;of the maze &nbsp;( N x M).</p>
<p>Second line of the input contains 'k' as described above .</p>
<p>The third line denotes the coordinates of the starting point ( 1-n ) , ( 1-m ) .</p>
<p>The next N lines contain the description of the Nth row .</p>
<h3>Output</h3>
<p>Output "YES" if it's possible .&nbsp;</p>
<p>Else output "NO" .</p>
<pre><strong>Constraints:<br>1&lt;=N,M&lt;=100</strong></pre>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 5</pre>
<pre>14</pre>
<pre>1 2</pre>
<pre>. . . * *</pre>
<pre>* . . . *</pre>
<pre>* . . . .</pre>
<pre>. * . . .</pre>
<pre>. * . . *</pre>
<pre><strong>Output:</strong>
YES<br><strong><br></strong>&nbsp;<strong><span style="font-size: x-large;">Explanation of the test case :<br>1,2 - 2,2 - 3,2 - 3,3 - 4,3 - 5,3 - 5,4 - 4,4 - 4,5 - 3,5 - 3,4 - 2,4 - 2,3 - 1,3 - 1,2 <br><br><span style="font-size: small;">14 moves were made ( No. of dashes ( - )) .<br>So , its possible . Also , no blocks were repeated . <br></span></span></strong></pre>