<p>&nbsp;</p>
<pre>|-------|    |-------|    |-------|    <br>|       |    |       |    |   |   |    <br>|---O   |    |---O   |    |   O   |          <br>|       |    |       |    |       |           <br>|-------|    |-------|    |-------|    <br>    A            B            C<br><br>|-------|    |-------|    |-------|<br>|       |    |       |    |       |<br>|   O   |    |   O   |    |   O   |<br>|   |   |    |   |   |    |   |   |<br>|-------|    |-------|    |-------|<br>    D            E            F<br><br>|-------|    |-------|    |-------|<br>|       |    |       |    |       |<br>|   O   |    |   O---|    |   O   |<br>|   |   |    |       |    |   |   |<br>|-------|    |-------|    |-------|  (Figure 1)<br>    G            H            I<br></pre>
<hr>
<p>There are nine clocks in a 3*3 array (figure 1). The goal is to return all the dials to 12 o'clock with as few moves as possible. There are nine different allowed ways to turn the dials on the clocks. Each such way is called a move. Select for each move a number 1 to 9. That number will turn the dials 90' (degrees) clockwise on those clocks which are affected according to figure 2 below.</p>
<pre>Move   Affected clocks<br> <br> 1         ABDE<br> 2         ABC<br> 3         BCEF<br> 4         ADG<br> 5         BDEFH<br> 6         CFI<br> 7         DEGH<br> 8         GHI<br> 9         EFHI    (Figure 2)<br></pre>
<h3>Input</h3>
<p>&nbsp;</p>
<p>Read nine numbers from standard input<kbd></kbd>. These numbers give the start positions of the dials. 0=12 o'clock, 1=3 o'clock, 2=6 o'clock, 3=9 o'clock. The example in figure 1 gives the following input data file:</p>
<pre>3 3 0<br>2 2 2 <br>2 1 2<br></pre>
<h3>Output</h3>
<p>&nbsp;</p>
<p>Write to the standard output the shortest sequence of moves (numbers), which returns all the dials to 12 o'clock. In case there are many solutions, write the solution which is the least in lexicographic order. In our example the <kbd>output</kbd> is as follows:</p>
<pre>4 5 8 9<br></pre>
<h3>Example</h3>
<pre>Each number represents a time accoring to following table:<br><pre>0 = 12 o'clock<br>1 = 3 o'clock<br>2 = 6 o'clock <br>3 = 9 o'clock<br></pre>
<br>
<pre>3 3 0         3 0 0         3 0 0          0 0 0         0 0 0 <br>2 2 2   5-&gt;   3 3 3   8-&gt;   3 3 3   4 -&gt;   0 3 3   9-&gt;   0 0 0 <br>2 1 2         2 2 2         3 3 3          0 3 3         0 0 0 <br><br>Note: This just represents a valid sequence of moves, and not the solution<br></pre>
<br></pre>