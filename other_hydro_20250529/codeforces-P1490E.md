## Description

<div><p>A championship is held in Berland, in which $n$ players participate. The player with the number $i$ has $a_i$ ($a_i \ge 1$) tokens.</p><p>The championship consists of $n-1$ games, which are played according to the following rules:</p><ul> <li> in each game, two random players with non-zero tokens are selected; </li><li> the player with more tokens is considered the winner of the game (in case of a tie, the winner is chosen randomly); </li><li> the winning player takes all of the loser's tokens; </li></ul><p>The last player with non-zero tokens is the winner of the championship.</p><p>All random decisions that are made during the championship are made equally probable and independently.</p><p>For example, if $n=4$, $a = [1, 2, 4, 3]$, then one of the options for the game (there could be other options) is: </p><ul> <li> during the first game, the first and fourth players were selected. The fourth player has more tokens, so he takes the first player's tokens. Now $a = [0, 2, 4, 4]$; </li><li> during the second game, the fourth and third players were selected. They have the same number of tokens, but in a random way, the third player is the winner. Now $a = [0, 2, 8, 0]$; </li><li> during the third game, the second and third players were selected. The third player has more tokens, so he takes the second player's tokens. Now $a = [0, 0, 10, 0]$; </li><li> the third player is declared the winner of the championship. </li></ul><p>Championship winners will receive personalized prizes. Therefore, the judges want to know in advance which players have a chance of winning, i.e have a non-zero probability of winning the championship. You have been asked to find all such players. </p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case consists of one positive integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of players in the championship.</p><p>The second line of each test case contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the number of tokens the players have.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, print the number of players who have a nonzero probability of winning the championship. On the next line print the numbers of these players in <span class="tex-font-style-bf">increasing</span> order. Players are numbered starting from one in the order in which they appear in the input. </p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case consists of one positive integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of players in the championship.</p><p>The second line of each test case contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the number of tokens the players have.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, print the number of players who have a nonzero probability of winning the championship. On the next line print the numbers of these players in <span class="tex-font-style-bf">increasing</span> order. Players are numbered starting from one in the order in which they appear in the input. </p>

## Samples

```input1
2
4
1 2 4 3
5
1 1 1 1 1
```

```output1
3
2 3 4 
5
1 2 3 4 5
```



