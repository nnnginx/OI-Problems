<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Brian the Computer Science Nerd is going on a date with his girlfriend, Anatevka! His romantic location of choice is a movie theatre - but not an IMAX theatre, of course, as that would be far too expensive.</p>
<p>This theatre has $10^9$ rows of $1000$ seats each, which are initially empty. The rows are numbered $1..10^9$ starting from the one closest to the screen, and the seats in each row are numbered $1..1000$ from left to right. Seat $c$ in row $r$ is denoted as seat ($r$, $c$). Seats in rows $1..L$ ($1 \leq L \leq 1000$) are considered to be "close" to the screen, while seats in further rows are considered to be "far".</p>
<p>Over the course of $T$ ($1 \leq T \leq 500,000$) minutes before the movie starts, a number of events occur. During the $i$th minute, either a person enters and sits in the empty seat ($R_i$, $C_i$), the person sitting in the occupied seat ($R_i$, $C_i$) leaves, or Anatevka suggests that she and Brian take seats ($R_i$, $C_i$) and ($R_i$, $C_i+1$). The type of the $i$th event is represented by the character $E_i$, with $E_i =$ "<strong>E</strong>" indicating a person entering, $E_i =$ "<strong>L</strong>" indicating a person leaving, and $E_i =$ "<strong>S</strong>" indicating a seating suggestion. All seats involved in the events are valid seats inside the theatre, and every seat that Anatevka suggests will be "close", as she believes that they're the best.</p>
<p>Every time Anatevka makes a suggestion, Brian must, of course, analyze its quality. If either of the two seats she suggests are already occupied, he should explain that her recommendation is invalid with a simple "No". Otherwise, he'd like to calculate the total inconvenience of both seats in such an arrangement. The inconvenience of sitting in seat ($r$, $c$) is the number of occupied seats in its field of vision (excluding itself). The field of vision of seat ($r$, $c$) includes all seats which are no further than it from seat ($1$, $c$) by Manhattan distance, as shown below (with the "S" representing a suggested seat, and an "F" representing a seat within its field of vision):</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:rmovie1.bmp" alt=""></p>
<p>After all of the events have taken place, the movie is about to start, and a final decision must be made on where to sit - and Brian will handle that. He concludes that seats that are "far" are clearly superior (as they offer a broader view of the screen), and he knows that the point of going to the movies is to have an optimal viewing experience, so selecting two adjacent seats is certainly not mandatory. As such, he'd like to determine the minimum total inconvenience for any two "far", unoccupied seats in the theatre. Note that, if one of the chosen seats is in the other's field of vision, this does not count towards its inconvenience - it's only determined by other people sitting in the theatre.</p>
<h3>Input</h3>
<p>First line: 2 integers, $L$ and $T$</p>
<p>Next $T$ lines: 1 character, $E_i$, and 2 integers, $R_i$ and $C_i$, for $i = 1..T$</p>
<h3>Output</h3>
<p>1 line for each of Anatevka's suggestions: If the suggestion is invalid, the string "No" - otherwise, the total inconvenience of the two suggested seats</p>
<p>Final line: The minimum total inconvenience of any pair of "far", unoccupied seats</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3 7<br>E 1 2<br>E 2 5<br>S 3 3<br>E 2 3<br>L 2 5<br>S 1 3<br>S 2 2</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3<br>0<br>No<br>0</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>When Anatevka makes her first suggestion, the front 3 rows and leftmost 5 columns of the theatre look as follows (where a "P" represents a person, and an "S" represents one of the suggested seats):</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:rmovie2.bmp" alt=""></p>
<p>The person sitting in seat ($1$, $2$) is in the field of vision of both suggested seats, while the person sitting in seat ($2$, $5$) is only in the way of the right one. As such, the total inconvenience of the two seats is $1+2=3$.</p>
<p>The second suggestion is shown below:</p>
<p style="text-align: center;"><img src="../../../content/sourspinach:rmovie3.bmp" alt=""></p>
<p>These two seats aren't obstructed by any people, so their total inconvenience is $0$. The final suggestion is invalid, as one of its two seats (seat ($2$, $3$)) is already occupied.</p>
<p>Finally, Brian can easily select two "far" which each have inconvenience $0$, as the theatre has $10^9-3$ "far" rows with $1000$ seats each, and most are far from the two people setting in the theatre after the last event. For example, he might choose to take seat ($4$, $6$), while recommending that Anatevka enjoy the view from seat ($100$, $1000$).</p>