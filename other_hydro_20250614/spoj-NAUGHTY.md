<p><span style="font-size: small;"> Mr. Naughty likes to play with balls. So his friend, Mr Nice, gave him <strong>n</strong> balls to play a game. Each ball has exactly two numbers (the number on the top   and the number on the bottom). In one move Mr Naughty can rotate any ball so   that its bottom now becomes the top. Mr Nice knows the minimum number of such   moves that can make at least half of the balls show same number on their top.   So to win Mr Nice's game, Mr Naughty should figure out the minimum number of   moves. Its not always possible to make such moves that satisfy the given   condition.In this case Mr Naughty should figure out that it is <strong>"Impossible"</strong> to   make such moves.</span></p>
<p><span style="font-size: small;"> Help Mr Naughty to win the game. </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> The first line contains a single integer <strong>n</strong> - the number of balls. The   following <strong>n</strong> lines contain the description of all balls, one ball per line.   Each description has a pair of non-negative integers not exceeding <strong>10^5</strong> -   numbers on top and bottom. The first number in a line is the number on top,   the second one - on the bottom. The number on the top of the ball may be same   as the number on the bottom.<br> The numbers in the lines are separated by single spaces. </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> On a single line print a single integer - the minimum number of moves to win   the game. If it is impossible to make the set funny, print <strong>"Impossible"</strong> (quotes for clarity). </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 1 ¡Ü n ¡Ü 10^5</strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">3
3 100
100 3
5 4</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">1</span></pre>
<h3><span style="font-size: small;">Explanation:</span></h3>
<p><span style="font-size: small;"> In this case Mr Naughty can rotate the first ball so that number on the top   becomes 100. Since two of the three balls have same number on their top (100),   you do not need to change anything else, so the answer is 1. </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">5 
5 9
5 9
3 2
1 4
5 7</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">0</span></pre>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">3
1 2
3 4
5 6 </span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">Impossible</span></pre>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Prateek Sachdev</strong></span></p>