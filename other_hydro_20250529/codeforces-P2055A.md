## Description

<div><center><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small"><span class="tex-font-style-it">Roaming through the alligator-infested Everglades, Florida Man encounters a most peculiar showdown.</span></span></td></tr></tbody></table></center><p>There are $n$ lilypads arranged in a row, numbered from $1$ to $n$ from left to right. Alice and Bob are frogs initially positioned on distinct lilypads, $a$ and $b$, respectively. They take turns jumping, starting with Alice. </p><p>During a frog's turn, it can jump either one space to the left or one space to the right, as long as the destination lilypad exists. For example, on Alice's first turn, she can jump to either lilypad $a-1$ or $a+1$, provided these lilypads are within bounds. It is important to note that each frog <span class="tex-font-style-bf">must jump</span> during its turn and cannot remain on the same lilypad.</p><p>However, there are some restrictions:</p><ul> <li> The two frogs cannot occupy the same lilypad. This means that Alice cannot jump to a lilypad that Bob is currently occupying, and vice versa. </li><li> If a frog cannot make a valid jump on its turn, it loses the game. As a result, the other frog wins. </li></ul><p>Determine whether Alice can guarantee a win, assuming that both players play optimally. It can be proven that the game will end after a finite number of moves if both players play optimally.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first and only line of each test case contains three integers $n$, $a$, and $b$ ($2 \leq n \leq 100$, $1 \leq a, b \leq n$, $a\neq b$)&nbsp;¡ª the number of lilypads, and the starting positions of Alice and Bob, respectively.</p><p>Note that there are <span class="tex-font-style-bf">no</span> constraints on the sum of $n$ over all test cases.</p></div><div class="output-specification"><p>For each test case, print a single line containing either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", representing whether or not Alice has a winning strategy. </p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first and only line of each test case contains three integers $n$, $a$, and $b$ ($2 \leq n \leq 100$, $1 \leq a, b \leq n$, $a\neq b$)&nbsp;¡ª the number of lilypads, and the starting positions of Alice and Bob, respectively.</p><p>Note that there are <span class="tex-font-style-bf">no</span> constraints on the sum of $n$ over all test cases.</p>

## Output

<p>For each test case, print a single line containing either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", representing whether or not Alice has a winning strategy. </p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,4,6
5
2 1 2
3 3 1
4 2 3
5 2 4
7 6 2
```




```output1
NO
YES
NO
YES
YES
```



## Note

<p>In the first test case, Alice has no legal moves. Therefore, Alice loses on the first turn.</p><p>In the second test case, Alice can only move to lilypad $2$. Then, Bob has no legal moves. Therefore, Alice has a winning strategy in this case.</p><p>In the third test case, Alice can only move to lilypad $1$. Then, Bob can move to lilypad $2$. Alice is no longer able to move and loses, giving Bob the win. It can be shown that Bob can always win regardless of Alice's moves; hence, Alice does not have a winning strategy.</p>
