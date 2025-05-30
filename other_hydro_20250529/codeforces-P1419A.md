## Description

<div><p>Everyone knows that agents in Valorant decide, who will play as attackers, and who will play as defenders. To do that Raze and Breach decided to play $t$ matches of a digit game...</p><p>In each of $t$ matches of the digit game, a positive integer is generated. It consists of $n$ digits. The digits of this integer are numerated from $1$ to $n$ from the highest-order digit to the lowest-order digit. After this integer is announced, the match starts.</p><p>Agents play in turns. Raze starts. In one turn an agent can choose any unmarked digit and mark it. Raze can choose digits on odd positions, but can not choose digits on even positions. Breach can choose digits on even positions, but can not choose digits on odd positions. The match ends, when there is only one unmarked digit left. If the single last digit is odd, then Raze wins, else Breach wins.</p><p>It can be proved, that before the end of the match (for every initial integer with $n$ digits) each agent has an ability to make a turn, i.e. there is at least one unmarked digit, that stands on a position of required parity.</p><p>For each of $t$ matches find out, which agent wins, if both of them want to win and play optimally.</p></div><div class="input-specification"><p>First line of input contains an integer $t$ $(1 \le t \le 100)$ &nbsp;�� the number of matches.</p><p>The first line of each match description contains an integer $n$ $(1 \le n \le 10^3)$ &nbsp;�� the number of digits of the generated number.</p><p>The second line of each match description contains an $n$-digit positive integer without leading zeros.</p></div><div class="output-specification"><p>For each match print $1$, if Raze wins, and $2$, if Breach wins.</p></div>

## Input

<p>First line of input contains an integer $t$ $(1 \le t \le 100)$ &nbsp;�� the number of matches.</p><p>The first line of each match description contains an integer $n$ $(1 \le n \le 10^3)$ &nbsp;�� the number of digits of the generated number.</p><p>The second line of each match description contains an $n$-digit positive integer without leading zeros.</p>

## Output

<p>For each match print $1$, if Raze wins, and $2$, if Breach wins.</p>

## Samples

```input1
4
1
2
1
3
3
102
4
2069
```

```output1
2
1
1
2
```




## Note

<p>In the first match no one can make a turn, the only digit left is $2$, it's even, so Breach wins.</p><p>In the second match the only digit left is $3$, it's odd, so Raze wins.</p><p>In the third match Raze can mark the last digit, after that Breach can only mark $0$. $1$ will be the last digit left, it's odd, so Raze wins.</p><p>In the fourth match no matter how Raze plays, Breach can mark $9$, and in the end there will be digit $0$. It's even, so Breach wins.</p>
