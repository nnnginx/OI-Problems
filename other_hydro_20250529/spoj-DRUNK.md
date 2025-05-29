<p><span style="font-size: small;"> Alice and Bob were getting bored and decided to play a game. The game involves   a pile of coins. Both players take turns in picking a certain number of coins   from the pile. Initially, the pile contains <strong>N</strong> coins. Alice makes the first   move. The player who is unable to pick up any coins in his/her turn loses the   game. Some of the details of the game are:</span></p>
<p><span style="font-size: small;"><br></span></p>
<ol>
<li><span style="font-size: small;">In each turn a player can only decide on picking up <strong>1, 4, 9, 16</strong> coins from the   pile.</span></li>
<span style="font-size: small;"><br> </span>
<li><span style="font-size: small;">As both the players are drunk and not in complete control of their actions,   even if they decide on picking up some coins, they might end up picking   something else completely. So, if a person decides on picking up <strong>X</strong> coins from   the pile, he/she might end up with <strong>(X - 1), X or (X + 1)</strong> coins with the   relative probability of<strong> C1: C2: C3</strong></span></li>
<span style="font-size: small;"><br> </span>
<li><span style="font-size: small;">In each turn a player has to eventually pick up at least <strong>1</strong> coin.</span></li>
</ol>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">Note that a player cannot decide on picking up <strong>X</strong> coins from the pile if the   pile contains less than <strong>X</strong> coins at the time. Also, if a player decided on   picking up <strong>X</strong> coins and it happens that picking up <strong>(X + 1)</strong> is not valid (This   might happen if there are only <strong>X</strong> coins in the pile), then the relative   probability distribution for the valid moves will be <strong>C1: C2</strong>. Similarly, if   picking up <strong>(X - 1)</strong> coins is not valid, then the relative probability   distribution for the valid moves will be <strong>C2: C3</strong>.</span></p>
<p><span style="font-size: small;"> As both of them are not in their right minds, they sometimes want to win and   sometimes want to lose. But Bob still wonders what is his probability of   winning/losing the game (depending on what he wants for a particular game).   Help him find out his probability! </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> The first line of the input contains a single integer, <strong>T</strong>, which represents the   number of test cases. Each test case contains <strong>3</strong> lines. The first line of each   test contains a single integer, <strong>N</strong>, which represents the number of coins in the   pile initially. The second line contains 3 integers <strong>C1, C2 and C3</strong>. The last   line of each test contains <strong>2</strong> integers describing the mood of Alice and Bob   respectively. <strong>0</strong> is for losing and <strong>1</strong> is for winning. </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> For each test cases, the probability of winning/losing (depending on the test   case) rounded to <strong>4</strong> places of precision. </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 1 ¡Ü T ¡Ü 10<br> 1 ¡Ü N ¡Ü 1000000<br> 1 ¡Ü  (C1,C2,C3) ¡Ü  100000<br></strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">2
1
1 2 3
0 0
5
1 2 3
0 1</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">1.0000
0.4333</span></pre>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Sukhjashan Singh</strong></span></p>