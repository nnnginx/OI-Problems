<p>Deal or No Deal is played in many different ways around the world. Many different countries have their own version or versions of the show, each with their own twists on the same general format. The general format is the following.
</p><p>The game revolves around the opening of a set of numbered briefcases, each of which contains a different prize (cash or otherwise). The contents of all of the cases are known at the start of the game, but the specific location of any prize is unknown. The value of each of the cases is indicated by a label or card sealed within it. The contestant claims (or is assigned) a case to begin the game. The case's value is not revealed until the conclusion of the game.
</p><p>The contestant then begins choosing cases to be removed from play. The amount inside each choice is immediately revealed; by process of elimination, the amount revealed cannot be inside the player's chosen case. Throughout the game, after a predetermined number of cases have been opened, the banker offers the contestant an amount of money and/or prizes to quit the game, the offer based roughly on the amounts remaining in play and the contestant's demeanor. The player then answers the titular question, choosing:
</p><ul>
<li>"Deal", accepting the offer presented and ending the game, or</li>
<li>"No Deal", rejecting the offer and continuing the game.</li>
</ul>
<p>This process of removing cases and receiving offers continues, until either the player accepts an offer to 'deal', or all offers have been rejected and the values of all unselected cases are revealed. The player wins the value of the deal taken, or if no deal is taken, the contents of the player's case.
</p><p>For the sake of this problem we will consider that the banker offers are deal before each removing of cases. Also we will assume that banker follows the particular model of contestants behaviour which is - if the banker offers the contestant the prize x the probability that the contestant accepts the deal is:</p><img src="./21247/file/I1GS6etw.png">,<p>
where min and max are the minimum and maximum prizes left in the game respectively. The banker wants to minimize the expexted prize the contestant wins. Help the banker calculate the expected prize the contestant is going to win if the banker offers optimal deals.

</p><h3>Input</h3>
<p>The first line of input is n - the number of briefcases. Next lines consists of n integers a<sub>1</sub>, a<sub>2</sub>, бн, a<sub>n</sub> - the prizes in the briefcases. Number q follows - the amount of situations the banker needs to evaluate. The description of each sitation follows: k иC the number of prizes still in the game; b<sub>1</sub>, b<sub>2</sub>, бн, b<sub>k</sub> иC the prizes themselves.

</p><h3>Constraints</h3>
<p>2 &lt;= n &lt;= 16<br>
1 &lt;= q &lt;= 100<br>
2 &lt;= k &lt;= n<br>
1 &lt;= a<sub>i</sub>, b<sub>i</sub> &lt;= 10<sup>6</sup>

</p><h3>Output</h3>
<p>For each situation print the expected prize the contestant is going to win and also the optimal deal the banker should offer. Both numbers should be printed with two digits after the dot.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
10 20 30 40
4
2 10 20
2 20 30
2 40 10
4 20 30 10 40

<b>Output:</b>
14.59 12.66
24.59 22.66
23.76 17.99
22.40 17.08

</pre>