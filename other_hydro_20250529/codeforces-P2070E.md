## Description

<div><p>Consider the following game. Two players have a binary string (a string consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>). The players take turns, the first player makes the first turn. During a player's turn, he or she has to choose exactly two adjacent elements of the string and remove them (<span class="tex-font-style-bf">the first element and the last element are also considered adjacent</span>). Furthermore, there are additional constraints depending on who makes the move:</p><ul> <li> if it's the first player's move, <span class="tex-font-style-bf">both</span> chosen characters should be <span class="tex-font-style-tt">0</span>; </li><li> if it's the second player's move, <span class="tex-font-style-bf">at least one</span> of the chosen characters should be <span class="tex-font-style-tt">1</span>. </li></ul><p>The player who can't make a valid move loses the game. This also means that if the string currently has less than $2$ characters, the current player loses the game.</p><p>You are given a binary string $s$ of length $n$. You have to calculate the number of its substrings such that, if the game is played on that substring and both players make optimal decisions, the first player wins. In other words, calculate the number of pairs $(l, r)$ such that $1 \le l \le r \le n$ and the first player has a winning strategy on the string $s_l s_{l+1} \dots s_r$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The second line contains the string $s$, consisting of exactly $n$ characters. Each character of the string is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print one integer ¡ª the number of substrings such that, if the game is played on that substring, the first player wins.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$).</p><p>The second line contains the string $s$, consisting of exactly $n$ characters. Each character of the string is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print one integer ¡ª the number of substrings such that, if the game is played on that substring, the first player wins.</p>





```input1|
10
0010010011
```




```output1
12
```



## Note

<p>In the first example, the following substrings are winning for the first player ($s[l:r]$ denotes $s_l s_{l+1} \dots s_r$):</p><ul> <li> $s[1:2]$; </li><li> $s[1:3]$; </li><li> $s[1:7]$; </li><li> $s[2:4]$; </li><li> $s[2:8]$; </li><li> $s[3:5]$; </li><li> $s[4:5]$; </li><li> $s[4:6]$; </li><li> $s[5:7]$; </li><li> $s[6:8]$; </li><li> $s[7:8]$; </li><li> $s[7:9]$. </li></ul>
