<style>
  .center-text-container {
    text-align: center;
  }

  .center-text-container > * {
    display: inline-block;
  }

  .example-table {
    text-align: left;
    margin-top: 10px;
    width: 100%;
  }

  .example-table td {
    vertical-align: top; 
  }

  .section {
    margin-top: 19px;
    margin-bottom:19px;
  }

  .paragraph {
    text-align: left;
    margin-top: 10px;
    margin-bottom: 10px;
  }

  .paragraph ul, .paragraph ol {
    margin-top: 3px;
    margin-bottom: 3px;
  }
</style>

<div class="section">
  <h3>Description</h3>
  <div class="paragraph">
    Consider the following common single-player game.
  </div>
  <div class="paragraph">
    A board has fifteen holes, arranged in a triangular pattern. Pegs fit in these holes.
  </div>
  <div class="paragraph">
    A valid move is to take a peg and jump in a straight line over an adjacent peg to the an empty hole two positions away from the starting position. The peg that was jumped is removed from the board. The player wins the game when there is only one peg remaining.
  </div>
  <div class="paragraph">
For example, in the game below, the player wins in two moves.
    <div class="center-text-container">
<pre>    x             .            .
   x .           . .          . .
  . . .   =&gt;    x . .   =&gt;   . . .
 . x . .       . x . .      . . . .
. . . . .     . . . . .    . . x . .</pre>
    </div>
  </div>
  <div class="paragraph">
    In the game below, the player has no possible moves and loses.
    <div class="center-text-container">
<pre>    x
   . .
  x . .
 . . . .
. . . . .
</pre>
    </div>
  </div>
  <div class="paragraph">
    Given a starting position, determine if it is possible to win.    
  </div>
</div>

<div class="section">
  <h3>Input</h3>
  <div class="paragraph">
    The first line is N, the number of starting pegs (0 &lt; N &lt; 15).
  </div>
  <div class="paragraph">
    The next N lines are the pegs' positions. The positions on the board are numbered as following:
    <div class="center-text-container">
<pre>        1
      2   3
    4   5   6
  7   8   9  10
11  12  13  14  15
</pre>
    </div>
  </div>
</div>

<table class="section example-table">
  <tbody><tr>
    <th>Input</th>
    <th>Input</th>
    <th>Input</th>
  </tr>
  <tr>
    <td>
<pre>3
1
2
8</pre>
    </td>
    <td>
<pre>14
2
3
4
5
6
7
8
9
10
11
12
13
14
15</pre>
    </td>
    <td>
<pre>13
2
3
13
5
8
11
10
9
12
4
14
15
13</pre>
    </td>
  </tr>
  <tr>
    <th>Output</th>
    <th>Output</th>
    <th>Output</th>
  </tr>
  <tr>
    <td>
<pre>yes</pre>
    </td>
    <td>
<pre>yes</pre>
    </td>
    <td>
<pre>yes</pre>
    </td>
  </tr>
</tbody></table>