## Description

<div><p>Phoenix has collected $n$ pieces of gold, and he wants to weigh them together so he can feel rich. The $i$-th piece of gold has weight $w_i$. All weights are <span class="tex-font-style-bf">distinct</span>. He will put his $n$ pieces of gold on a weight scale, one piece at a time. </p><p>The scale has an unusual defect: if the total weight on it is <span class="tex-font-style-bf">exactly</span> $x$, it will explode. Can he put all $n$ gold pieces onto the scale in some order, without the scale exploding during the process? If so, help him find some possible order. </p><p>Formally, rearrange the array $w$ so that for each $i$ $(1 \le i \le n)$, $\sum\limits_{j = 1}^{i}w_j \ne x$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \le n \le 100$; $1 \le x \le 10^4$)&nbsp;！ the number of gold pieces that Phoenix has and the weight to avoid, respectively. </p><p>The second line of each test case contains $n$ space-separated integers $(1 \le w_i \le 100)$&nbsp;！ the weights of the gold pieces. It is guaranteed that the weights are <span class="tex-font-style-bf">pairwise distinct</span>.</p></div><div class="output-specification"><p>For each test case, if Phoenix cannot place all $n$ pieces without the scale exploding, print <span class="tex-font-style-tt">NO</span>. Otherwise, print <span class="tex-font-style-tt">YES</span> followed by the rearranged array $w$. If there are multiple solutions, print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \le n \le 100$; $1 \le x \le 10^4$)&nbsp;！ the number of gold pieces that Phoenix has and the weight to avoid, respectively. </p><p>The second line of each test case contains $n$ space-separated integers $(1 \le w_i \le 100)$&nbsp;！ the weights of the gold pieces. It is guaranteed that the weights are <span class="tex-font-style-bf">pairwise distinct</span>.</p>

## Output

<p>For each test case, if Phoenix cannot place all $n$ pieces without the scale exploding, print <span class="tex-font-style-tt">NO</span>. Otherwise, print <span class="tex-font-style-tt">YES</span> followed by the rearranged array $w$. If there are multiple solutions, print any.</p>

## Samples

```input1
3
3 2
3 2 1
5 3
1 2 3 4 8
1 5
5
```

```output1
YES
3 2 1
YES
8 1 2 3 4
NO
```




## Note

<p>In the first test case, Phoenix puts the gold piece with weight $3$ on the scale first, then the piece with weight $2$, and finally the piece with weight $1$. The total weight on the scale is $3$, then $5$, then $6$. The scale does not explode because the total weight on the scale is never $2$.</p><p>In the second test case, the total weight on the scale is $8$, $9$, $11$, $14$, then $18$. It is never $3$.</p><p>In the third test case, Phoenix must put the gold piece with weight $5$ on the scale, and the scale will always explode.</p>
