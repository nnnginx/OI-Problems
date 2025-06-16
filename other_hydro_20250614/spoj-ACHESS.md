<p>The world of the Adventurous Chess Masters is quite different than our world, instead of having streets and buildings everything is composed of a big chess board and chess pieces. A square of a chess board is said to be covered if at least one chess piece is placed on it. The mysteries of the world can be revealed by covering special magical squares over the chess board, and you can't wait to discover them.</p>
<p>In every turn you can update the board by moving one of the pieces on the board according to the following rules:</p>
<ul>
<li>The <strong>king</strong> moves only one square in any direction.</li>
<li>The <strong>queen</strong> moves any number of squares in any direction along a row, column, or diagonal.</li>
<li>The <strong>rook</strong> moves any number of squares along rows or columns (forward, backward, left or right).</li>
<li>The <strong>bishop</strong> moves any number of squares diagonally.</li>
<li>The <strong>knight</strong> moves to a square in an "L"-shape (two spaces forward, backward, left, or right and one space perpendicular to it).</li>
<li>The <strong>pawn</strong> can only move one space forward or backward (unlike a chess game).\</li>
</ul>
<p>Note that, unlike normal chess, more than one piece can occupy the same square and pieces can move through occupied squares. To reveal the secrets of the world you have to make the maximum number of magical squares covered, in the minimum number of turns.</p>
<p><strong>Input Specification:</strong></p>
<p>The first line of input contains an integer T that represents the number of test cases, then follow T test cases. The first line of each test case contains P and L, the number of chess pieces on the board and the number of magical squares in order.&nbsp; Following the first line P lines each contains two integers x and y coordinates of the location of the piece where (1 �� x, y �� 8) and the type of the chess pieces (king, queen, rook, bishop, knight, or pawn��all in small letters) and the last L lines of the test case each contains a unique pair of integers x and y as the coordinates of the magical squares where (1 �� x, y �� 8). Note that: (0 �� P �� 64), and these P pieces won't be in any of the L given locations.</p>
<p>&nbsp;</p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, print on one line ��<strong>Case K: </strong>Secret reveals after moving H pieces with minimum number of moves M.�� Where K is test case number, H is the number of pieces to be moved and M is the total number of moves used. Check Sample below to see the format.<strong> </strong></p>
<p><strong>Sample input:</strong></p>
<p>2<br>1 1<br>1 1 pawn<br>8 1<br>3 5<br>2 8 king<br>2 8 queen<br>7 5 bishop<br>1 1<br>2 2<br>3 6<br>6 3<br>4 4</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: Secret reveals after moving 1 pieces with minimum number of moves 7.<br>Case 2: Secret reveals after moving 3 pieces with minimum number of moves 5.</p>