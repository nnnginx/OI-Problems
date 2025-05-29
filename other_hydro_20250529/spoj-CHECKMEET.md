The white king George lives all alone in a <a href="https://en.wikipedia.org/wiki/Chessboard"> chessboard </a> (A standard chessboard consists of <strong>8</strong> rows and columns). He lives alone because the evil black king Andrew killed all the other pieces in frustration after George beat him in a game of chess.

<br><br>

Wandering all alone with no purpose and literally bored to death, King George invented a new game to keep him occupied. King George has a <i>secret word</i> in his mind. It is the word he used to shout instead of the usual <i>checkmate</i> after beating the black king in a chess game. King George loves to march, so he decided to take a tour through the chessboard. He assigns a single lowercase letter to each square of the chessboard first. He can then start his tour from any square on the chessboard. From a square, the king can move to any neighboring square inside the board as in the game of <a href="https://en.wikipedia.org/wiki/Chess"> chess </a>. However, it is not allowed to move to the same square twice during the journey. In other words, all the squares visited by the king must be <strong>distinct</strong>.

<br><br>

After completing his tour (the tour can be stopped anytime), George concatenates all the characters in the order of his travel to form a word. Since he has nothing better to do, the white king wants to know how many different ways he can complete the tour so that the secret word is formed afterward.

<br><br>

Two ways are considered different if a different square is visited at any moment. Note that the order in which the squares are visited also matters. As a consequence, for example the path <strong>(1, 2) -&gt; (2, 1)</strong> and <strong>(2, 1) -&gt; (1, 2)</strong> are considered different.

<br><br>

Formally the problem is as follows:
<br><br>

Let <strong>B(X, Y)</strong> be the lowercase letter assigned to square <strong>(X, Y)</strong>. Also, let the <i>secret word</i> be <strong>S<sub>1</sub> S<sub>2</sub> ... S<sub>K</sub></strong>.
Your task is to find the number of possible <i>King's tours</i>. A King's tour is a sequence of coordinates <strong>(X<sub>1</sub>, Y<sub>1</sub>), (X<sub>2</sub>, Y<sub>2</sub>), ... , (X<sub>K</sub>, Y<sub>K</sub>)</strong> satisfying:

<br><br>

<strong><li>1 ¡Ü X<sub>i</sub>, Y<sub>i</sub> ¡Ü 8</li></strong>
<strong><li>B(X<sub>i</sub>, Y<sub>i</sub>) = S<sub>i</sub> for all 1 ¡Ü i ¡Ü K</li></strong>
<strong><li> (X<sub>i</sub>, Y<sub>i</sub>) ¡Ù (X<sub>j</sub>, Y<sub>j</sub>) for all 1 ¡Ü i &lt; j ¡Ü K </li></strong>
<strong><li>max(|X<sub>i</sub> - X<sub>i + 1</sub>|, |Y<sub>i</sub> - Y<sub>i + 1</sub>|) = 1 for all 1 ¡Ü i &lt; K </li></strong>

<br><br>

<h3>Input</h3>
The first line of input consists of a single integer <strong>K</strong> denoting the length of the secret word. The next line contains the secret word consisting of <strong>K</strong> lowercase letters. The next <strong>8</strong> lines each contain <strong>8</strong> characters describing the lowercase letters assigned to the chessboard in row-major order.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü K ¡Ü 11</li></strong>

<h3>Output</h3>
Print a single line containing a single integer denoting the number of different tours forming the secret word.

<h3>Sample Input</h3>
<pre>2
aa
aabbbbbb
aabbbbbb
bbbbbbbb
bbbbbbbb
bbbbbbbb
bbbbbbbb
bbbbbbbb
bbbbbbbb
</pre>

<h3>Sample Output</h3>
<pre>12

</pre>


<h3>Sample Input</h3>
<pre>9
checkmate
checkmat
checkmee
checkmat
checkmee
checkmat
checkmee
checkmat
checkmee
</pre>

<h3>Sample Output</h3>
<pre>7698
</pre>
<br><br>

<h3>Reference</h3>
<a href="https://www.hackerrank.com/contests/university-codesprint-3/challenges/march-of-the-king">HackerRank - March Of The King</a>