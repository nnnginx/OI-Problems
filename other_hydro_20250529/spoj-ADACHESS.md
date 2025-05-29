<p>Ada the Ladybug was playing <a href="https://en.wikipedia.org/wiki/Chess_piece">chess</a> agains her good friend Velvet Mite Vinit. They were talking to each other during the game, saying "I will take your <em>figure</em> in next <strong>X</strong> moves". After the game, this was really bugging Ada so she have decided to give it more thinking.</p>
<p>As she can't determine it "that fast", she asked you to make a program which could output the minimal number of moves in which two figures could get to each other (note they they don't have to alternate, so all the moves could be done only by one of the figeres). Also note that it is classical <strong>8x8</strong> chessboard.</p>
<p>The interesting figures will be: <strong>King, Knight, Queen, Tower, Bishop</strong></p>
<h3>Input</h3>
<p>The first line of input will contain <strong> 1 ¡Ü T ¡Ü     3*10<sup>5</sup></strong>, the number of test-cases.</p>
<p>Each of the testcases will contain 6 integers <strong>f x y F X Y</strong>, where <strong>0 ¡Ü f, F ¡Ü 4 </strong> are the types of figures (0 to 4 standing for <strong>King, Knight, Queen, Tower, Bishop</strong> in this order) and <strong>0 ¡Ü x y X Y ¡Ü 7</strong>, the coordinates of given figures.</p>
<h3>Output</h3>
<p>For each test-case output the minimal number of moves get both figures to same "box". In case the figures can't meet, output "<strong>INF</strong>".</p>
<h3>Example Input</h3>
<pre>5
1 0 0 1 7 7
2 1 3 3 2 5 
0 1 0 4 5 5
3 1 1 4 3 3
0 1 2 0 3 4
</pre>
<h3>Example Output</h3>
<pre>6
2
2
1
2
</pre>
<h3>Example Input</h3>
<pre>10
2 3 6 1 6 2
3 3 6 3 6 7
4 4 6 4 2 4
3 6 0 4 1 0
3 7 1 3 5 2
0 0 6 1 5 4
0 5 7 3 3 5
0 4 1 4 5 3
3 2 1 3 4 2
0 5 2 0 2 7
</pre>
<h3>Example Output</h3>
<pre>2
2
1
1
2
3
2
2
2
5
</pre>