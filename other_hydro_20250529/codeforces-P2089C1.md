## Description

<div><p>  </p><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is that in this version, it is guaranteed that $k=0$. You can hack only if you solved all versions of this problem.</span> </p><p>A toy box is a refrigerator filled with childhood delight. Like weakness, struggle, hope ... When such a sleeper is reawakened, what kind of surprises will be waiting?</p><p>M received her toy box as a birthday present from her mother. A jewellery designer would definitely spare no effort in decorating yet another priceless masterpiece as a starry firmament with exquisitely shaped gemstones. In addition, $l$ distinct locks secure the tiny universe of her lovely daughter: a hair clip featuring a flower design, a weathered feather pen, a balloon shaped like the letter M ... each piece obscures a precious moment.</p><p>A few days ago, M rediscovered her toy box when she was reorganizing her bedroom, along with a ring of keys uniquely designed for the toy box. Attached to the key ring are $(l + k)$ keys, of which $l$ keys are able to open one of the $l$ locks correspondingly, while the other $k$ keys are nothing but counterfeits to discourage brute-force attack. To remind the correspondence, M's mother adorned each key with a gemstone of a different type. However, passing days have faded M's memory away.</p><p>"... So I have to turn to you all," M said while laying that ring of keys on the table.</p><p>K picked up the keys and examined them carefully. "The appearance of these keys unveils nothing fruitful. Thus, I am afraid that we shall inspect them sequentially."</p><p>Although everyone is willing to help M, nobody has a plan. Observing others' reactions, T suggested, "Let's play a game. Everyone tries a key in turn, and who opens the most locks is <span class="tex-font-style-it">amazing</span>."</p><p>$n$ members, including M herself, take turns to unlock the toy box recursively in the same order until all the $l$ locks are unlocked. At each turn, the current member only selects a single key and tests it on exactly one of the locks. To open the toy box as soon as possible, every member chooses the key and the lock that maximize the probability of being a successful match. If there are multiple such pairs, a member will randomly choose one of such pairs with equal probability. Apparently, if a lock has been matched with a key, then neither the lock nor the key will be chosen again in following attempts.</p><p>Assume that at the very beginning, the probability that a lock can be opened by any key is equal. If everyone always tries the optimal pairs of keys and locks based on all the historical trials, what will the expected number of successful matches be for each member?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The only line of the input contains three integers, $n$, $l$, $k$ ($1 \leq n \leq 100, 1 \leq l \leq 5000, k = 0$)&nbsp;�� the number of members participating in the game, the number of locks, and the number of counterfeit keys.</p><p>It is guaranteed that the sum of $l$ across all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, output a single line with $n$ integers $e_1, \ldots, e_n$, where $e_i$ represents the expected number of successful matches, modulo $10^9 + 7$.</p><p>Formally, let $M = 10^9 + 7$. It can be shown that the exact answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $e_i$ that $0 \le x &lt; M$ and $e_i \cdot q \equiv p \pmod{M}$. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The only line of the input contains three integers, $n$, $l$, $k$ ($1 \leq n \leq 100, 1 \leq l \leq 5000, k = 0$)&nbsp;�� the number of members participating in the game, the number of locks, and the number of counterfeit keys.</p><p>It is guaranteed that the sum of $l$ across all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, output a single line with $n$ integers $e_1, \ldots, e_n$, where $e_i$ represents the expected number of successful matches, modulo $10^9 + 7$.</p><p>Formally, let $M = 10^9 + 7$. It can be shown that the exact answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $e_i$ that $0 \le x &lt; M$ and $e_i \cdot q \equiv p \pmod{M}$. </p>





```input1|2,4
4
3 1 0
3 2 0
2 5 0
9 104 0
```




```output1
1 0 0
500000004 1 500000004
200000004 800000008
869203933 991076635 39374313 496894434 9358446 51822059 979588764 523836809 38844739
```



## Note

<p>For the first test case, there is only $1$ lock, so the first member opens the only lock with the only key undoubtedly.</p><p>For the second test case, there are exactly $2$ locks and $2$ keys, with each key corresponding to one of the locks. Without extra information, the first member randomly chooses a key and a lock with equal probabilities, for which the probability of success is $1/2$.</p><ul> <li> If the first member succeeds, the second member will open the other lock with the other key. </li><li> If the first member fails, then the key she selected can open the other lock, and the other key must correspond to the lock she chose. This information allows both the second and the third member to open a lock. </li></ul><p>In conclusion, the expected numbers of successful matches will be:</p><p>$$ \begin{split} e_1 &amp;= \frac{1}{2}\times 1 + \frac{1}{2}\times 0 = \frac{1}{2} \equiv 500,000,004 \pmod {10^9+7},\\ e_2 &amp;= \frac{1}{2}\times 1 + \frac{1}{2} \times 1 = 1,\\ e_3 &amp;= \frac{1}{2}\times 0 + \frac{1}{2} \times 1 = \frac{1}{2} \equiv 500,000,004\pmod {10^9+7}. \end{split} $$</p>
