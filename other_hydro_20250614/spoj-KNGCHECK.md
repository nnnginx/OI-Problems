<p style="margin: 0px 0px 1em; font-family: verdana; font-size: 14px; line-height: 21px;">Chess is a two-player strategy board game played on a chessboard, a square checkered game board with 64 squares arranged in an eight-by-eight grid. It is one of the world's most popular games, played by millions of people worldwide at home, in clubs, online, by correspondence, and in tournaments. Each player begins the game with 16 pieces: one king, one queen, two rooks, two knights, two bishops, and eight pawns. Each of the six piece types moves differently. Pieces are used to attack and capture the opponent's pieces, with the objective to 'checkmate' the opponent's king by placing it under an inescapable threat of capture. In addition to checkmate, the game can be won by the voluntary resignation of the opponent, which typically occurs when too much material is lost, or if checkmate appears unavoidable. A game may also result in a draw in several ways, where neither player wins. The course of the game is divided into three phases: opening, middle game, and endgame. Source Wikipedia</p>
<p style="margin: 0px 0px 1em; font-family: verdana; font-size: 14px; line-height: 21px;">To simplify this problem you will only deal with Kings, Knights and Pawns of the Black and the White Players. Assume that the White Player starts at the lower half of the board and the Black Player starts at the upper half. Given the state of the board, your task is to determine whether the black king is checked or not. For Clarity a 'Check' occurs when the King's square can be attacked by any of the opponent's pieces for his next move, and note that in this problem we will ignore the consequences which will follow, we don¡¯t even care whose turn is now but only consider the board state (out of chess rules).</p>
<p style="margin: 0px 0px 1em; font-family: verdana; font-size: 14px; line-height: 21px;">The Knight moves like an "L", it moves from cell (r1, c1) to cell (r2, c2) if and only if (r1 - r2)<sup>2</sup>&nbsp;+ (c1-c2)<sup>2</sup>&nbsp;= 5 (8 possible moves).</p>
<p style="margin: 0px 0px 1em; font-family: verdana; font-size: 14px; line-height: 21px;">The King can move only one move in its four main directions and its four diagonals (8 possible moves).</p>
<p style="margin: 0px 0px 1em; font-family: verdana; font-size: 14px; line-height: 21px;">The Pawn attacks only one move diagonally and only to the oppenent direction (2 possible moves).</p>
<p style="margin: 0px 0px 1em; font-family: verdana; font-size: 14px; line-height: 21px;">This problem is <strong>NOT</strong> following all chess rules, for example in real chess third case in the sample is INVALID, so please assume that the given board is always valid, just check the black king state.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p><span style="font-family: verdana; font-size: 14px; line-height: 21px;">You are given an 8x8 Board with Chess Pieces denoted as following: BK = Black King, WK = White King, BH = Black Knight, WH = White Knight, BP = Black Pawn, WP = White Pawn. We ensure that there is one and only one Black King in the Chess Board. Blank fields are denoted by ¡°-¡±. Cases are seperated by blank lines.</span></p>
<h3>Output</h3>
<p><span style="font-family: verdana; font-size: 14px; line-height: 21px;">You should output ¡°Check¡± if a Check exists or ¡°Not Check¡± if no check exists. Follow the output format described in the sample tests.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3
- - - - - - - -
- - - - - - - -
- - - - - - - -
- BH - - - - - -
- - - BK - - - -
- - WP - - - - -
- - - - - - - -
- - - - - - - -

- - - - - - - -
BH - - BH - - - -
- - - - - - - -
- - - - - - - -
- - - BK - - - -
- - - - - - - -
- WP - - - - WH -
- - - WK - - - -

- - - - - - - -
- - - - - - - -
- - - - - - - -
- - - - - - - -
- - - BK - - - -
- - - WK - - - -
- - - - - - WH -
- - - - - - - -
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 642px; width: 1px; height: 1px; overflow: hidden;">- WP - - - - WH -</div><strong>Output:</strong>
Case #1: Check
Case #2: Not Check
Case #3: Check<span style="white-space: normal;">
</span></pre>