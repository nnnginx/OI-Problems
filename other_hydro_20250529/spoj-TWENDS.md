<p>
In the two-player game ¡°Two Ends¡±, an even number of cards is laid out in a row. On each card, face
up, is written a positive integer. Players take turns removing a card from either end of the row and
placing the card in their pile. The player whose cards add up to the highest number wins the game.
Now one strategy is to simply pick the card at the end that is the largest ¡ª we¡¯ll call this the greedy
strategy. However, this is not always optimal, as the following example shows: (The first player would
win if she would first pick the 3 instead of the 4.)

</p><p></p><p>
3 2 10 4

</p><p></p><p>
You are to determine exactly how bad the greedy strategy is for different games when the second player
uses it but the first player is free to use any strategy she wishes.

</p><h3>Input</h3>
<p>
There will be multiple test cases. Each test case will be contained on one line. Each line will start with
an even integer n followed by n positive integers. A value of <i>n</i> = 0 indicates end of input. You may
assume that <i>n</i> is no more than 1000. Furthermore, you may assume that the sum of the numbers in
the list does not exceed 1,000,000.

</p><h3>Output</h3>
<p>
For each test case you should print one line of output of the form:

</p><p></p><p>
<b><i>In game m, the greedy strategy might lose by as many as p points.</i></b>

</p><p></p><p>
where <i>m</i> is the number of the game (starting at game 1) and <i>p</i> is the maximum possible difference
between the first player¡¯s score and second player¡¯s score when the second player uses the greedy strategy.
When employing the greedy strategy, always take the larger end. If there is a tie, remove the left end.

</p><h3>Example</h3>

<pre><b>Input:</b>
4 3 2 10 4
8 1 2 3 4 5 6 7 8
8 2 2 1 5 3 8 7 3
0

<b>Output:</b>
In game 1, the greedy strategy might lose by as many as 7 points.
In game 2, the greedy strategy might lose by as many as 4 points.
In game 3, the greedy strategy might lose by as many as 5 points.
</pre>