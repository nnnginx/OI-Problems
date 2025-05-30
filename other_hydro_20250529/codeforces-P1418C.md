## Description

<div><p>You and your friend are playing the game Mortal Kombat XI. You are trying to pass a challenge tower. There are $n$ bosses in this tower, numbered from $1$ to $n$. The type of the $i$-th boss is $a_i$. If the $i$-th boss is easy then its type is $a_i = 0$, otherwise this boss is hard and its type is $a_i = 1$.</p><p>During one session, either you or your friend can kill <span class="tex-font-style-bf">one or two</span> bosses (neither you nor your friend can skip the session, so the minimum number of bosses killed during one session is at least one). After your friend session, your session begins, then again your friend session begins, your session begins, and so on. <span class="tex-font-style-bf">The first session is your friend's session</span>.</p><p>Your friend needs to get good because he can't actually kill hard bosses. To kill them, he uses skip points. One skip point can be used to kill one hard boss.</p><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> number of skip points your friend needs to use so you and your friend kill all $n$ bosses in the given order.</p><p>For example: suppose $n = 8$, $a = [1, 0, 1, 1, 0, 1, 1, 1]$. Then the best course of action is the following:</p><ul> <li> your friend kills two first bosses, using one skip point for the first boss; </li><li> you kill the third and the fourth bosses; </li><li> your friend kills the fifth boss; </li><li> you kill the sixth and the seventh bosses; </li><li> your friend kills the last boss, using one skip point, so the tower is completed using two skip points. </li></ul><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) �� the number of bosses. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 1$), where $a_i$ is the type of the $i$-th boss.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer: the <span class="tex-font-style-bf">minimum</span> number of skip points your friend needs to use so you and your friend kill all $n$ bosses in the given order.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) �� the number of bosses. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 1$), where $a_i$ is the type of the $i$-th boss.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer: the <span class="tex-font-style-bf">minimum</span> number of skip points your friend needs to use so you and your friend kill all $n$ bosses in the given order.</p>

## Samples

```input1
6
8
1 0 1 1 0 1 1 1
5
1 1 1 1 0
7
1 1 1 1 0 0 1
6
1 1 1 1 1 1
1
1
1
0
```

```output1
2
2
2
2
1
0
```



