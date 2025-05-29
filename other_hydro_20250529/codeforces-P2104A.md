## Description

<div><p>Monocarp placed three decks of cards in a row on the table. The first deck consists of $a$ cards, the second deck consists of $b$ cards, and the third deck consists of $c$ cards, with the condition $a &lt; b &lt; c$.</p><p>Monocarp wants to take some number of cards (at least one, but no more than $c$) from the <span class="tex-font-style-bf">third</span> deck and distribute them between the first two decks so that each of the taken cards ends up in either the first or the second deck. It is possible that all the cards taken from the third deck will go into the same deck.</p><p>Your task is to determine whether Monocarp can make the number of cards in all three decks equal using the described operation.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains three integers $a, b$, and $c$ ($1 \le a, b, c \le 10^8$)&nbsp;！ the number of cards in the first, second, and third decks, respectively.</p><p>Additional constraint on the input: $a &lt; b &lt; c$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Monocarp can make the number of cards in all three decks equal using the described operation. Otherwise, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains three integers $a, b$, and $c$ ($1 \le a, b, c \le 10^8$)&nbsp;！ the number of cards in the first, second, and third decks, respectively.</p><p>Additional constraint on the input: $a &lt; b &lt; c$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Monocarp can make the number of cards in all three decks equal using the described operation. Otherwise, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1|2,4
4
3 5 10
12 20 30
3 5 7
1 5 6
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first test case, Monocarp has to take $4$ cards from the third deck, put $3$ cards in the first deck, and $1$ card in the second deck. Thus, there will be $6$ cards in all three decks.</p><p>In the second test case, it is impossible to make the number of cards in all three decks equal.</p><p>In the third test case, Monocarp has to take $2$ cards from the third deck and put both in the first deck. Thus, there will be $5$ cards in all three decks.</p><p>In the fourth test case, it is also impossible to make the number of cards in all three decks equal.</p>
