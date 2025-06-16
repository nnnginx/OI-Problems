<div>
<p>Let's imagine: there is a chess piece <span>billiard ball</span>.  Its movements resemble the ones of a bishop chess piece. The only  difference is that when a billiard ball hits the board's border, it can  reflect from it and continue moving.</p>
<p>More formally, first one of  four diagonal directions is chosen and the billiard ball moves in that  direction. When it reaches the square located on the board's edge, the  billiard ball reflects from it; it changes the direction of its movement  by 90 degrees and continues moving. Specifically, having reached a  corner square, the billiard ball is reflected twice and starts to move  the opposite way. While it moves, the billiard ball can make an infinite  number of reflections. At any square of its trajectory the billiard  ball can stop and on that the move is considered completed.</p>
<img src="./21550/file/TZUuOYk8.png" alt="">
<p>It is considered that one billiard ball <span><em>a</em></span> beats another billiard ball <span><em>b</em></span> if <span><em>a</em></span> can reach a point where <span><em>b</em></span> is located.</p>
<p>You  are suggested to find the maximal number of billiard balls, that  pairwise do not beat each other and that can be positioned on a  chessboard <span><em>n</em> × <em>m</em></span> in size.</p>
</div>
<h3>Input</h3>
<pre>The first line of input contains two integers <span><em>n</em></span> and <span><em>m</em></span> (<span>2 ≤ <em>n</em>, <em>m</em> ≤ 10<sup>16</sup></span>).</pre>
<h3>Output</h3>
<pre>Print a single line for each input line containing a single number, the maximum possible number of billiard balls that do not pairwise beat each other.</pre>
<h3>Example</h3>
<pre><strong>Input:<br>3 4<br>2 2<br>5 5<br></strong><strong><br>Output:</strong><br>2<br>2<br>5</pre>