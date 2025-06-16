<p><span style="font-size: small;">Nowadays, gamble is so familiar even though it is prohibited in some countries. There are so many ways to gamble. Every rules of gambling always include the probability to win the game. Here, there is a unique rule of a gamble. This rule is called Cyclic Counting Gamble. This game is played by N players and there is only one winner. Those N players are standing and making a big circle. They are numbered from 1 to N. One player is pointed to be number one. Then, player who is in right side of the player numbered i, become player number i+1 (for 1 ¡Ü i &lt; N). To decide who is the winner, they will chose one number K, then the following algorithm is used :<br><br></span></p>
<ol>
<li><span style="font-size: small;">Starting from player number one, saying "one" (1)</span></li>
<li><span style="font-size: small;">Then, right side of player who is saying i, will say i+1</span></li>
<li><span style="font-size: small;">Repeat the second rule until a player saying K</span></li>
<li><span style="font-size: small;">That player will be considered to be lose, get out from circle and can't play anymore</span></li>
<li><span style="font-size: small;">Player who is right side of that lose player will say "one" and back to second rule</span></li>
<li><span style="font-size: small;">Repeat that algorithm until one player left, that player become the only winner</span></li>
</ol>
<p><span style="font-size: small;"><br>Now, N players want to join that gamble (N is given). Then, they already chose K. Because N and K is too large, then the game can't finished although one century. Here, you are to find the fastest algorithm to know the winner in less than 0.5 second.</span></p>
<p><span style="font-size: small;"> </span></p>
<h3><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">Given N and K in one line separated by a white space.</span></p>
<p><span style="font-size: small;"> </span></p>
<h3><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">The only line contain one number represent the winner of that game.</span></p>
<h3><span style="font-size: small;">Constraint<br></span></h3>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">1 ¡Ü N , K ¡Ü 10<sup>18</sup></span></p>
<p><span style="font-size: small;">N <span style="font-size: small;">¡Ü 10<sup>7</sup> or K <span style="font-size: small;">¡Ü 10<sup>5</sup><br></span></span></span></p>
<p><span style="font-size: small;"> </span></p>
<h3><span style="font-size: small;">Example</span></h3>
<p><span style="font-size: small;"> </span></p>
<pre><span style="font-size: small;"><strong>Input:</strong>
5 2

<strong>Output:</strong>
3<br></span></pre>
<h3><span style="font-size: small;">Explanation<br></span></h3>
<p><span style="font-size: small;">Sequence of players who are saying :</span></p>
<pre><span style="font-size: small;">1 say 1<br><strong>2</strong> say 2 (lose)<br>3 <span style="font-size: small;">say 1<br></span><strong>4</strong> <span style="font-size: small;">say 2 <span style="font-size: small;">(lose)<br></span></span>5 <span style="font-size: small;">say 1<br></span><strong>1</strong> <span style="font-size: small;">say 2 <span style="font-size: small;">(lose)<br></span></span>3 <span style="font-size: small;">say 1<br></span><strong>5</strong><span style="font-size: small;"> say 2<span style="font-size: small;"> (lose)</span></span></span></pre>
<p><span style="font-size: small;"><span style="font-size: small;">&nbsp;</span>The winner is player with number 3.</span></p>