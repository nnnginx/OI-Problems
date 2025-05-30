## Description

<div><p>You are asked to watch your nephew who likes to play with toy blocks in a strange way.</p><p>He has $n$ boxes and the $i$-th box has $a_i$ blocks. His game consists of two steps: </p><ol> <li> he chooses an arbitrary box $i$; </li><li> he tries to move <span class="tex-font-style-bf">all</span> blocks from the $i$-th box to other boxes. </li></ol> If he can make the same number of blocks in each of $n - 1$ other boxes then he will be happy, otherwise, will be sad. Note that your nephew can only move the blocks from the chosen box to the other boxes; he cannot move blocks from the other boxes.<p>You don't want to make your nephew sad, so you decided to put several extra blocks into some boxes in such a way that no matter which box $i$ he chooses he won't be sad. What is the minimum number of extra blocks you need to put?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains the integer $n$ ($2 \le n \le 10^5$)&nbsp;！ the number of boxes.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ the number of blocks in each box.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum number of blocks you need to put. It can be proved that the answer always exists, i.&nbsp;e. the number of blocks is finite.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains the integer $n$ ($2 \le n \le 10^5$)&nbsp;！ the number of boxes.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ the number of blocks in each box.</p><p>It's guaranteed that the sum of $n$ over test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum number of blocks you need to put. It can be proved that the answer always exists, i.&nbsp;e. the number of blocks is finite.</p>

## Samples

```input1
3
3
3 2 2
4
2 2 3 2
3
0 3 0
```

```output1
1
0
3
```




## Note

<p>In the first test case, you can, for example, put one extra block into the first box and make $a = [4, 2, 2]$. If your nephew chooses the box with $4$ blocks, then we will move two blocks to the second box and two blocks to the third box. If he chooses the box with $2$ blocks then he will move these two blocks to the other box with $2$ blocks.</p><p>In the second test case, you don't need to put any extra blocks, since no matter which box your nephew chooses, he can always make other boxes equal.</p><p>In the third test case, you should put $3$ extra blocks. For example, you can put $2$ blocks in the first box and $1$ block in the third box. You'll get array $a = [2, 3, 1]$.</p>
