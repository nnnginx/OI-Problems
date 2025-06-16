## Description

<div><p>Alice and Bob are playing a game in an array $a$ of size $n$.</p><p>They take turns to do operations, with Alice starting first. The player who can not operate will lose. At first, a variable $mx$ is set to $0$.</p><p>In one operation, a player can do:</p><ul><li> Choose an index $i$ ($1 \le i \le n$) such that $a_{i} \geq mx$ and set $mx$ to $a_{i}$. Then, set $a_{i}$ to $0$.</li></ul><p>Determine whether Alice has a winning strategy.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>For each test case: </p><ul> <li> The first line contains an integer $n$ ($2 \leq n \leq 50$)&nbsp;！ the size of the array. </li><li> The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;！ the elements of the array. </li></ul></div><div class="output-specification"><p>For each test case, if Alice has a winning strategy, output "<span class="tex-font-style-tt">YES</span>". Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>For each test case: </p><ul> <li> The first line contains an integer $n$ ($2 \leq n \leq 50$)&nbsp;！ the size of the array. </li><li> The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;！ the elements of the array. </li></ul>

## Output

<p>For each test case, if Alice has a winning strategy, output "<span class="tex-font-style-tt">YES</span>". Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11
5
2
2 1
2
1 1
3
3 3 3
4
3 3 4 4
4
1 2 2 2
```




```output1
YES
NO
YES
NO
YES
```



## Note

<p>In the first test case, Alice can choose $i=1$ since $a_1=2 \ge mx=0$.</p><p>After Alice's operation, $a=[0,1]$ and $mx=2$. Bob can not do any operation. Alice wins.</p><p>In the second test case, Alice doesn't have a winning strategy.</p><p>For example, if Alice chooses $i=1$, after Alice's operation: $a=[0,1]$ and $mx=1$. Then, Bob can choose $i=2$ since $a_2=1 \ge mx=1$. After Bob's operation: $a=[0,0]$ and $mx=1$. Alice can not do any operation. Bob wins.</p>
