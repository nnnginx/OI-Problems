## Description

<div><p> </p><p>There are $n$ monsters, numbered from $1$ to $n$, in front of Gellyfish. The HP of the $i$-th monster is $h_i$.</p><p>Gellyfish doesn't want to kill them, but she wants to keep these monsters from being a threat to her. So she wants to reduce the HP of all the monsters to exactly $1$.</p><p>Now, Gellyfish, with The Sword Sharpened with Tears, is going to attack the monsters for $m$ rounds. For each round:</p><ol> <li> The Sword Sharpened with Tears shines with a probability of $p$. </li><li> Gellyfish can choose whether to attack: <ul> <li> If Gellyfish doesn't attack, nothing happens. </li><li> If Gellyfish chooses to attack and The Sword Sharpened with Tears shines, the HP of all the monsters will be reduced by $1$. </li><li> If Gellyfish chooses to attack and The Sword Sharpened with Tears does not shine, Gellyfish can choose one of the monsters and reduce its HP by $1$. </li></ul> </li></ol><p>Please note that before Gellyfish decides whether or not to attack, she will know whether the sword shines or not. Also, when the sword shines, Gellyfish can only make attacks on all the monsters and cannot make an attack on only one monster.</p><p>Now, Gellyfish wants to know what the probability is that she will reach her goal if she makes choices optimally during the battle.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $p'$ ($1 \leq n \leq 20$, $1 \leq m \leq 4000$, $0 \leq p' \leq 100$)&nbsp;！ the number of monsters, the number of rounds of attacks, and an integer representing the probability $p = \frac {p'} {100}$ that the Sword Sharpened with Tears shines.</p><p>The second line of each test case contains $n$ integers $h_1,h_2,\ldots,h_n$ ($1 \leq h_i \leq 400$)&nbsp;！ the HP of the monsters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p></div><div class="output-specification"><p>For each test case, output a single real number representing the probability that Gellyfish will reach her goal.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-6}$. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $p'$ ($1 \leq n \leq 20$, $1 \leq m \leq 4000$, $0 \leq p' \leq 100$)&nbsp;！ the number of monsters, the number of rounds of attacks, and an integer representing the probability $p = \frac {p'} {100}$ that the Sword Sharpened with Tears shines.</p><p>The second line of each test case contains $n$ integers $h_1,h_2,\ldots,h_n$ ($1 \leq h_i \leq 400$)&nbsp;！ the HP of the monsters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p>

## Output

<p>For each test case, output a single real number representing the probability that Gellyfish will reach her goal.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-6}$. </p>





```input1|2,3,6,7
4
2 2 10
2 2
5 5 20
2 2 2 2 2
6 20 50
1 1 4 5 1 4
9 50 33
9 9 8 2 4 4 3 5 3
```




```output1
0.910000
0.672320
0.588099
0.931474
```



## Note

<p>In the first test case, Gellyfish will always attack whether the sword shines or not in the first round.</p><p>If the sword shines in the first round, then Gellyfish can reach her goal after the attack in the first round.</p><p>Otherwise, if the sword does not shine in the first round, she will attack monster $1$ in the first round. For the second round:</p><ul> <li> If the sword shines, since monster $1$ was attacked in the first round, Gellyfish can't reach her goal. </li><li> Otherwise, Gellyfish can attack monster $2$, allowing her to reach her goal. </li></ul><p>Therefore, the probability that Gellyfish can reach her goal is $10\% + (90\% \cdot 90\%) = 91\%$.</p><p>In the second test case, Gellyfish will only attack in the first round where the sword shines. It can be observed that the only way Gellyfish can't reach her goal is if the sword never shines in all $5$ rounds. The probability that Gellyfish can reach her goal is $100\% - (80\%)^5 = 67.232\%$.</p>
