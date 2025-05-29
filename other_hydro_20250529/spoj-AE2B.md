<p>
  Bytean chess is one of the most peculiar variants of chess in the world.
  Playing each match is a major difficulty, because the game is played on an infinite chessboard.
  The basic ability learnt by young enthusiasts of Bytean chess is considering
  all possible situations on a chessboard after millions of moves.
  To perform this, they need to know whether a given chess piece can get from one given square to another one.
</p>
<p>
  The most powerful chess piece in Bytean chess is a (K, N)-knight.
  Its moves resemble the moves of a knight in traditional chess.
  Each of its moves consists of: either moving K squares vertically
  and afterwards N squares horizontally, or moving N squares vertically and afterwards
  K squares horizontally.
  The knight from traditional chess can therefore be thought of as (2, 1)-knight or
  (1, 2)-knight.

</p>
<p>
  The task is to verify, for two given squares of the chessboard, if a (K, N)-knight can get
  from the first square to the second one (the number of necessary moves is not important).
</p>
    <h2>Input</h2>
<p>
  The first line of the standard input contains one integer T
  (1 ¡Ü T ¡Ü 20000) denoting the number of test cases.
  Each of the following T lines contains a description of a single test case
  in the form of six integers K, N, x<sub>1</sub>, y<sub>1</sub>, x<sub>2</sub>, y<sub>2</sub>

  (0 ¡Ü K, N ¡Ü 10<sup>9</sup>, K + N &gt; 0, -10<sup>9</sup> ¡Ü x<sub>1</sub>, y<sub>1</sub>, x<sub>2</sub>, y<sub>2</sub> ¡Ü 10<sup>9</sup>)
  separated by single spaces.
  K and N describe the possible moves of the knight.
  The knight starts its movement in square (x<sub>1</sub>, y<sub>1</sub>). We would like to check if it can get to square (x<sub>2</sub>, y<sub>2</sub>).
  </p>
	
    <h2>Output</h2>
    <p>

  For each test case exactly one line should be written to the standard output.
  It should contain a word <tt>TAK</tt> (meaning YES) or <tt>NIE</tt> (meaning NO)
  depending on whether a (K, N)-knight starting from square (x<sub>1</sub>, y<sub>1</sub>)
  can get to square (x<sub>2</sub>, y<sub>2</sub>).
</p>

<h2>Example</h2>

<p>For the input data:</p><pre>3
2 1 0 0 3 3
1 1 1 1 1 2
1 0 2 3 4 6</pre>
<p>the correct result is:</p><pre>TAK
NIE
TAK</pre>

<p><i>Task author: Jakub Onufry Wojtaszczyk.</i></p>