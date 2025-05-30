## Description

<div><p>Omkar has a pie tray with $k$ ($2 \leq k \leq 20$) spots. Each spot in the tray contains either a chocolate pie or a pumpkin pie. However, Omkar does not like the way that the pies are currently arranged, and has another ideal arrangement that he would prefer instead.</p><p>To assist Omkar, $n$ elves have gathered in a line to swap the pies in Omkar's tray. The $j$-th elf from the left is able to swap the pies at positions $a_j$ and $b_j$ in the tray.</p><p>In order to get as close to his ideal arrangement as possible, Omkar may choose a contiguous subsegment of the elves and then pass his pie tray through the subsegment starting from the left. However, since the elves have gone to so much effort to gather in a line, they request that Omkar's chosen segment contain at least $m$ ($1 \leq m \leq n$) elves.</p><p>Formally, Omkar may choose two integers $l$ and $r$ satisfying $1 \leq l \leq r \leq n$ and $r - l + 1 \geq m$ so that first the pies in positions $a_l$ and $b_l$ will be swapped, then the pies in positions $a_{l + 1}$ and $b_{l + 1}$ will be swapped, etc. until finally the pies in positions $a_r$ and $b_r$ are swapped.</p><p>Help Omkar choose a segment of elves such that the amount of positions in Omkar's final arrangement that contain the same type of pie as in his ideal arrangement is the maximum possible. <span class="tex-font-style-bf">Note that since Omkar has a big imagination, it might be that the amounts of each type of pie in his original arrangement and in his ideal arrangement do not match</span>.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $k$ ($1 \leq m \leq n \leq 10^6$ and $2 \leq k \leq 20$) &nbsp;�� the number of elves, the minimum subsegment length, and the number of spots in Omkar's tray respectively. </p><p>The second and third lines each contain a string of length $k$ consisting of $0$s and $1$s that represent initial arrangement of pies and ideal arrangement of pies; the $j$-th character in each string is equal to $0$ if the $j$-th spot in the arrangement contains a chocolate pie and is equal to $1$ if the $j$-th spot in the arrangement contains a pumpkin pie. It is not guaranteed that the two strings have the same amount of $0$s or the same amount of $1$s.</p><p>$n$ lines follow. The $j$-th of these lines contains two integers $a_j$ and $b_j$ ($1 \leq a_j, b_j \leq k$, $a_j \neq b_j$) which indicate that the $j$-th elf from the left can swap the pies at positions $a_j$ and $b_j$ in the tray.</p></div><div class="output-specification"><p>Output two lines. </p><p>The first line should contain a single integer $s$ ($0 \leq s \leq k$) equal to the amount of positions that contain the same type of pie in Omkar's final arrangement and in Omkar's ideal arrangement; $s$ should be the maximum possible. </p><p>The second line should contain two integers $l$ and $r$ satisfying $1 \leq l \leq r \leq n$ and $r - l + 1 \geq m$, indicating that Omkar should pass his tray through the subsegment $l, l + 1, \dots, r$ to achieve a final arrangement with $s$ positions having the same type of pie as his ideal arrangement.</p><p>If there are multiple answers you may output any of them.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $k$ ($1 \leq m \leq n \leq 10^6$ and $2 \leq k \leq 20$) &nbsp;�� the number of elves, the minimum subsegment length, and the number of spots in Omkar's tray respectively. </p><p>The second and third lines each contain a string of length $k$ consisting of $0$s and $1$s that represent initial arrangement of pies and ideal arrangement of pies; the $j$-th character in each string is equal to $0$ if the $j$-th spot in the arrangement contains a chocolate pie and is equal to $1$ if the $j$-th spot in the arrangement contains a pumpkin pie. It is not guaranteed that the two strings have the same amount of $0$s or the same amount of $1$s.</p><p>$n$ lines follow. The $j$-th of these lines contains two integers $a_j$ and $b_j$ ($1 \leq a_j, b_j \leq k$, $a_j \neq b_j$) which indicate that the $j$-th elf from the left can swap the pies at positions $a_j$ and $b_j$ in the tray.</p>

## Output

<p>Output two lines. </p><p>The first line should contain a single integer $s$ ($0 \leq s \leq k$) equal to the amount of positions that contain the same type of pie in Omkar's final arrangement and in Omkar's ideal arrangement; $s$ should be the maximum possible. </p><p>The second line should contain two integers $l$ and $r$ satisfying $1 \leq l \leq r \leq n$ and $r - l + 1 \geq m$, indicating that Omkar should pass his tray through the subsegment $l, l + 1, \dots, r$ to achieve a final arrangement with $s$ positions having the same type of pie as his ideal arrangement.</p><p>If there are multiple answers you may output any of them.</p>

## Samples

```input1
4 2 5
11000
00011
1 3
3 5
4 2
3 4
```

```output1
5
1 3
```






```input2
4 3 5
11000
00011
1 3
1 5
2 4
1 5
```

```output2
3
1 4
```




## Note

<p>In the first test case, the swaps will go like this: </p><ul> <li> Swap $1$ and $3$: <span class="tex-font-style-tt">11000</span> becomes <span class="tex-font-style-tt">01100</span> </li><li> Swap $3$ and $5$: <span class="tex-font-style-tt">01100</span> becomes <span class="tex-font-style-tt">01001</span> </li><li> Swap $4$ and $2$: <span class="tex-font-style-tt">01001</span> becomes <span class="tex-font-style-tt">00011</span> </li></ul> The final arrangement is the same as the ideal arrangement <span class="tex-font-style-tt">00011</span>, so there are $5$ positions with the same type of pie, which is optimal.<p>In the second test case, the swaps will go like this: </p><ul> <li> Swap $1$ and $3$: <span class="tex-font-style-tt">11000</span> becomes <span class="tex-font-style-tt">01100</span> </li><li> Swap $1$ and $5$: <span class="tex-font-style-tt">01100</span> becomes <span class="tex-font-style-tt">01100</span> </li><li> Swap $4$ and $2$: <span class="tex-font-style-tt">01100</span> becomes <span class="tex-font-style-tt">00110</span> </li><li> Swap $1$ and $5$: <span class="tex-font-style-tt">00110</span> becomes <span class="tex-font-style-tt">00110</span> </li></ul> The final arrangement has $3$ positions with the same type of pie as the ideal arrangement <span class="tex-font-style-tt">00011</span>, those being positions $1$, $2$, and $4$. In this case the subsegment of elves $(l, r) = (2, 3)$ is more optimal, but that subsegment is only length $2$ and therefore does not satisfy the constraint that the subsegment be of length at least $m = 3$.
