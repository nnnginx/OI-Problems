<p>In the country of Rome, Chess is a royal game. For evey move the players had to give some bucks to the Emperor Jurg. The LGMs or Little Green Men, are very good player of chess. But as the chess is a expensive game, thats why it is royal, they asked you to help them find the minimum bucks which they had to pay for moving their Knight from one position to another. Any number of steps can be used to reach the destination.</p>
<p><strong>Constraints:</strong></p>
<p>The chess has a dimension of 8X8, and the index of left bottom cell (0, 0).</p>
<p>Knight move only in a standard way, i.e. 2 row and 1 col or 1 row and 2 col.</p>
<p>If in a step Knight move from (a, b) to (c, d), then LGM had to pay a*c + b*d bucks to Emperor Jurg.</p>
<p>0 ¡Ü a, b, c, d ¡Ü 7</p>
<h3>Input</h3>
<p>There are 100-150 test cases. Each test case is composed of four space separeated integers.The first two numbers, a, b, are the starting position of the Knight and the next two, c, d, are the destination of the Knight. Read upto End Of File.</p>
<h3>Output</h3>
<p>For each test case, print the minimum amount of bucks they had to pay in separate line. If its impossible to reach the destination then print -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2 5 5 2<br>4 7 3 2<br>1 2 3 4<br><br><strong>Output:</strong><br>42<br>78<br>18<br><br><br><em><span style="text-decoration: underline;">Explanation for test case #1:<br></span>2 5 5 2<br><br></em>For moving Knight from (2, 5) to (5, 2) in minimum cost,  one of the path is (2, 5) -&gt; (3, 3) -&gt;(5, 2)<br>Bucks paid:<br>(2, 5)              =  0<br>(2, 5) -&gt; (3, 3) =  0 + (2*3 + 5*3) = 21<br>(3, 3) -&gt; (5, 2) = 21 + (3*5 + 3*2) = 42<br>     <br><br><em>To infinity and beyond...</em><br></pre>