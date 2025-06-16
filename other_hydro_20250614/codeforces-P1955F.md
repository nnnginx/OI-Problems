## Description

<div><p>Alice and Bob gathered in the evening to play an exciting game on a sequence of $n$ integers, each integer of the sequence <span class="tex-font-style-bf">doesn't exceed $4$</span>. The rules of the game are too complex to describe, so let's just describe the winning condition ！ Alice wins if the <a href="http://tiny.cc/xor_wiki_eng">bitwise XOR</a> of all the numbers in the sequence is non-zero; otherwise, Bob wins.</p><p>The guys invited Eve to act as a judge. Initially, Alice and Bob play with $n$ numbers. After one game, Eve removes one of the numbers from the sequence, then Alice and Bob play with $n-1$ numbers. Eve removes one number again, after which Alice and Bob play with $n - 2$ numbers. This continues until the sequence of numbers is empty.</p><p>Eve seems to think that in such a game, Alice almost always wins, so she wants Bob to win as many times as possible. Determine the maximum number of times Bob can win against Alice if Eve removes the numbers optimally.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first and only line of each test case contains four integers $p_i$ ($0 \le p_i \le 200$)&nbsp;！ the number of ones, twos, threes, and fours in the sequence at the beginning of the game.</p></div><div class="output-specification"><p>For each test case, print the maximum number of times Bob will win in a separate line, if Eve removes the numbers optimally.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first and only line of each test case contains four integers $p_i$ ($0 \le p_i \le 200$)&nbsp;！ the number of ones, twos, threes, and fours in the sequence at the beginning of the game.</p>

## Output

<p>For each test case, print the maximum number of times Bob will win in a separate line, if Eve removes the numbers optimally.</p>





```input1|2,4,6
5
1 1 1 0
1 0 1 2
2 2 2 0
3 3 2 0
0 9 9 9
```




```output1
1
1
3
3
12
```



## Note

<p>In the first example, Bob wins when Eve has not removed any numbers yet.</p><p>In the second example, Bob wins if Eve removes one one and one three.</p>
