<p>When we were trying to solve the problem SDGAME, we got a misunderstanding of it.We didn't get AC until we were told the original meaning.But we think our kind of understanding is also interesting and is worthy of doing.So enjoy the problem.

</p><p>Alice and Bob are playing a game.  The game consists of a circular track of M (2 &lt;= M &lt;= 1,000,000,000) cells labeled 0 through M - 1.  Initially both players start at cell 0.  The game progresses by having each player take turns rolling one of N (1 &lt;= N &lt;= 10,000) 'super-dice' labeled 0 through N - 1.  The actual mechanics of the 'super-dice' is not very well understood; however, it is known that they will only ever turn up a number between 0 and 1,000,000,000 inclusive after a roll.  After rolling the super-dice the number of spaces a player moves is determined by the product of a contiguous subsequence of the values shown on the dice <b>(which are available)</b>(There are special rules for determining the range that vary each move that will not be discussed).<b>If all the values are unavailable,the player moves one space.Iff the number on the dice is more than 1,000,000,000 or less than 0, the dice is unavailable.</b>

</p><p>To make matters more complicated, after any turn if Alice and Bob land on the same cell the value shown on all dice<b>(neither available nor unavailable)</b> is multiplied by the label of the cell they are on.  Note in this way it is possible for some dice to show numbers greater than 1,000,000,000.

</p><p>After playing this game for a while, Alice and Bob have grown frustrated because the calculations became too difficult.  Given the series of R (1 &lt;= R &lt;= 100,000) dice rolls and ranges, help Alice and Bob determine their position after each move.  Assume that all dices start out showing 1 <b>and all dices are available</b>.

</p><h3>Input</h3>
<p>The first line contains R, N, and M each separated by a space.  R lines follow.  Each line will contain d v a b separated by a space.  d indicates the label of the dice rolled.  v indicates the value shown on the dice.  a and b indicate the range of dice used to determine the move distance.

</p><h3>Output</h3>
<p>R lines containing the position of the player that just rolled after their roll.


</p><h3>Example</h3>

<pre><b>Input:</b>
6 4 4
0 1000000000 1 1
1 999999998 1 1
2 500000000 3 3
0 1 2 2
3 1 0 3
0 6 0 3

<b>Output:</b>
1
2
2
2
0
0

<b>Output Explanation:</b>

For your assistance, here is the state of the dice after each turn:(* means unavailable)
Before all rolls:
[1,1,1,1](0,0)
After first roll:
[1000000000,1,1,1](1,0)
After second roll:
[1000000000,999999998,1,1](1,2)
After third roll:
[1000000000,999999998,500000000,1](2,2)
All dices multiply 2:
[*,*,1000000000,2](2,2)
After forth roll:
[1,*,1000000000,2](2,2)
All dices multiply 2:
[2,*,*,4](2,2)
After fifth roll:
[2,*,*,1](0,2)
After sixth roll:
[6,*,*,1](0,0)
All dices multiply 0:
[0,0,0,0](0,0)

<h3>Test data has been updated, all submissions have been rejudged</h3>
</pre>