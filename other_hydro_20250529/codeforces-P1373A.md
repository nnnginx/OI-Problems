## Description

<div><p>There are two rival donut shops.</p><p>The first shop sells donuts at retail: each donut costs $a$ dollars.</p><p>The second shop sells donuts only in bulk: box of $b$ donuts costs $c$ dollars. So if you want to buy $x$ donuts from this shop, then you have to buy the smallest number of boxes such that the total number of donuts in them is greater or equal to $x$.</p><p>You want to determine two <span class="tex-font-style-bf">positive integer</span> values: </p><ol> <li> how many donuts can you buy so that they are strictly cheaper in the first shop than in the second shop? </li><li> how many donuts can you buy so that they are strictly cheaper in the second shop than in the first shop? </li></ol><p>If any of these values doesn't exist then that value should be equal to $-1$. If there are multiple possible answers, then print any of them.</p><p><span class="tex-font-style-bf">The printed values should be less or equal to $10^9$. It can be shown that under the given constraints such values always exist if any values exist at all.</span></p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;�� the number of testcases.</p><p>Each of the next $t$ lines contains three integers $a$, $b$ and $c$ ($1 \le a \le 10^9$, $2 \le b \le 10^9$, $1 \le c \le 10^9$).</p></div><div class="output-specification"><p>For each testcase print two <span class="tex-font-style-bf">positive</span> integers. For both shops print such $x$ that buying $x$ donuts in this shop is strictly cheaper than buying $x$ donuts in the other shop. $x$ should be greater than $0$ and less or equal to $10^9$.</p><p>If there is no such $x$, then print $-1$. If there are multiple answers, then print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;�� the number of testcases.</p><p>Each of the next $t$ lines contains three integers $a$, $b$ and $c$ ($1 \le a \le 10^9$, $2 \le b \le 10^9$, $1 \le c \le 10^9$).</p>

## Output

<p>For each testcase print two <span class="tex-font-style-bf">positive</span> integers. For both shops print such $x$ that buying $x$ donuts in this shop is strictly cheaper than buying $x$ donuts in the other shop. $x$ should be greater than $0$ and less or equal to $10^9$.</p><p>If there is no such $x$, then print $-1$. If there are multiple answers, then print any of them.</p>

## Samples

```input1
4
5 10 4
4 5 20
2 2 3
1000000000 1000000000 1000000000
```

```output1
-1 20
8 -1
1 2
-1 1000000000
```




## Note

<p>In the first testcase buying any number of donuts will be cheaper in the second shop. For example, for $3$ or $5$ donuts you'll have to buy a box of $10$ donuts for $4$ dollars. $3$ or $5$ donuts in the first shop would cost you $15$ or $25$ dollars, respectively, however. For $20$ donuts you'll have to buy two boxes for $8$ dollars total. Note that $3$ and $5$ are also valid answers for the second shop, along with many other answers.</p><p>In the second testcase buying any number of donuts will be either cheaper in the first shop or the same price. $8$ donuts cost $32$ dollars in the first shop and $40$ dollars in the second shop (because you have to buy two boxes). $10$ donuts will cost $40$ dollars in both shops, so $10$ is not a valid answer for any of the shops.</p><p>In the third testcase $1$ donut costs $2$ and $3$ dollars, respectively. $2$ donuts cost $4$ and $3$ dollars. Thus, $1$ is a valid answer for the first shop and $2$ is a valid answer for the second shop.</p><p>In the fourth testcase $10^9$ donuts cost $10^{18}$ dollars in the first shop and $10^9$ dollars in the second shop.</p>
