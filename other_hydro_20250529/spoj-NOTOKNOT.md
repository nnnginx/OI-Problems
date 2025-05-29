<p>Disentangling of string loops is a classical 3D- puzzle. A designer of one of these puzzles wants
to know if two given string loops can be disentangled or not. <br> <br>
The designer says that a string loop configuration that can be disentangled is a Notknot. In
fact, he says that knots are those string loops that can not be disentangled. <br> <br>
Your task is to write a program to help the puzzle designer deciding if some configurations
can or cannot be disentangled. In the problems that you are going to solve, loops are defined by
straight segments in the space between points with integer coordinates. Then, a loop is described
with a list of p points with integral coordinates for some p ≥ 3. <br> <br>

</p><h3>Input</h3>
<p>Input consists of N test cases (1 ≤ N ≤ 1000). The number N is given in the first line of the input.<br><br> 
Each test case contains the description of two loops, each one in a line. A description for a p points loop (3 ≤ p ≤ 20) is given in one input line with 3p integer numbers separated by blanks:<br> <br></p><p></p><p>
</p><center> x1 y1 z1 x2 y2 z2 . . . xp yp zp </center>
<br><br><p></p><p>
    what represents the loop:<br><br></p><p></p><p>
                     </p><p> </p><center>(x1 , y1 , z1 ) − (x2 , y2 , z2 ) − · · · − (xp , yp , zp ) − (x1 , y1 , z1 )</center><br><br><p></p><p>
    where there is a straight segment between adjacent coordinates.<br>
</p><h3>Output</h3>
<p>For each analyzed case, one line classifying the case: Notknot or Knot.

</p><h3>Example</h3>
<pre><b>Input:</b>
3
10 0 0 0 0 -10 0 10 0 0 0 10
5 0 0 -10 -10 0 0 5 0 10 10 0
10 0 0 0 0 -10 0 10 0 0 0 10
15 0 0 -10 -10 0 0 5 0 10 10 0
1 0 0 0 1 0 0 0 1
10 10 0 0 10 0 0 0 10 10 0 0 25 5 0 3 3 0


<b>Output:</b>
Notknot
Knot
Notknot

</pre>