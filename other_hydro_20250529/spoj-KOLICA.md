<p>A number of shopping carts filled with explosives are floating in a coordinate system, in one of the four main directions (up, down, left or right). All carts are moving at a speed of one unit per second.</p>
<p>Movement is continuous; for example, in one third of a second, a cart travels one third of a unit.</p>
<p>When two or more carts collide (are at the same place at the same time), there is an explosion and all carts taking part in the collision explode and cease to exist.</p>
<p>Write a program that, given the starting points and directions of all carts, determines which carts never explode.</p>
<h3>Input</h3>
<p>The first line of input contains an integer N (2 ¡Ü N ¡Ü 500), the number of carts.</p>
<p>Each of the following N lines contains two integers and a string. Each pair of integers describes the starting coordinates of one cart (between 0 and 100 000 000, inclusive), and the string describes the direcction in which the cart is moving ("gore" for up, "dolje" for down, "lijevo" for left, or "desno" for right).</p>
<p>No two carts will start at the same coordinates.</p>
<h3>Output</h3>
<p>Output the indices of all carts which never explode, sorted in ascending order, one index per line. The first cart in the input is labeled 1, the second is labeled 2 etc. If no carts survive, output "nema".</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4<br>5 5 dolje<br>5 6 lijevo<br>5 7 desno<br>5 8 gore

<strong>Output:</strong>
1<br>2<br>3<br>4<br><strong><br><br>Input:</strong><br>5<br>3 3 dolje<br>1 1 desno<br>5 1 lijevo<br>100000 500000 desno<br>900000 500000 lijevo<br><br><strong>Output:</strong><br>nema<br><br><br><strong>Input:</strong><br>3<br>10 0 gore<br>0 10 desno<br>15 5 lijevo
<br><strong>Output:<br></strong>2<strong><br></strong></pre>