## Description

<div><p>Vova plans to go to the conference by train. Initially, the train is at the point $1$ and the destination point of the path is the point $L$. The speed of the train is $1$ length unit per minute (i.e. at the first minute the train is at the point $1$, at the second minute ！ at the point $2$ and so on).</p><p>There are lanterns on the path. They are placed at the points with coordinates divisible by $v$ (i.e. the first lantern is at the point $v$, the second is at the point $2v$ and so on).</p><p>There is also <span class="tex-font-style-bf">exactly</span> one standing train which occupies all the points from $l$ to $r$ inclusive.</p><p>Vova can see the lantern at the point $p$ if $p$ is divisible by $v$ and there is no standing train at this position ($p \not\in [l; r]$). Thus, if the point with the lantern is one of the points covered by the standing train, Vova can't see this lantern.</p><p>Your problem is to say the number of lanterns Vova will see during the path. Vova plans to go to $t$ different conferences, so you should answer $t$ <span class="tex-font-style-bf">independent</span> queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of queries.</p><p>Then $t$ lines follow. The $i$-th line contains four integers $L_i, v_i, l_i, r_i$ ($1 \le L, v \le 10^9$, $1 \le l \le r \le L$) ！ destination point of the $i$-th path, the period of the lantern appearance and the segment occupied by the standing train.</p></div><div class="output-specification"><p>Print $t$ lines. The $i$-th line should contain one integer ！ the answer for the $i$-th query.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of queries.</p><p>Then $t$ lines follow. The $i$-th line contains four integers $L_i, v_i, l_i, r_i$ ($1 \le L, v \le 10^9$, $1 \le l \le r \le L$) ！ destination point of the $i$-th path, the period of the lantern appearance and the segment occupied by the standing train.</p>

## Output

<p>Print $t$ lines. The $i$-th line should contain one integer ！ the answer for the $i$-th query.</p>

## Samples

```input1
4
10 2 3 7
100 51 51 51
1234 1 100 199
1000000000 1 1 1000000000

```

```output1
3
0
1134
0

```




## Note

<p>For the first example query, the answer is $3$. There are lanterns at positions $2$, $4$, $6$, $8$ and $10$, but Vova didn't see the lanterns at positions $4$ and $6$ because of the standing train.</p><p>For the second example query, the answer is $0$ because the only lantern is at the point $51$ and there is also a standing train at this point.</p><p>For the third example query, the answer is $1134$ because there are $1234$ lanterns, but Vova didn't see the lanterns from the position $100$ to the position $199$ inclusive.</p><p>For the fourth example query, the answer is $0$ because the standing train covers the whole path.</p>
