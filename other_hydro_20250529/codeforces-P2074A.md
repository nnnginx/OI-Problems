## Description

<div><p>The pink soldiers have given you $4$ <span class="tex-font-style-bf">distinct points</span> on the plane. The $4$ points' coordinates are $(-l,0)$, $(r,0)$, $(0,-d)$, $(0,u)$ correspondingly, where $l$, $r$, $d$, $u$ are positive integers.</p><center> <img class="tex-graphics" src="./36018/file/45bWBhPB.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">In the diagram, a square is drawn by connecting the four points $L$, $R$, $D$, $U$.</span> </center><p>Please determine if it is possible to draw a square$^{\text{∗}}$ with the given points as its vertices.</p><div class="statement-footnote"><p>$^{\text{∗}}$A <span class="tex-font-style-it">square</span> is defined as a polygon consisting of $4$ vertices, of which all sides have equal length and all inner angles are equal. No two edges of the polygon may intersect each other.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains four integers $l$, $r$, $d$, $u$ ($1 \le l,r,d,u \le 10$).</p></div><div class="output-specification"><p>For each test case, if you can draw a square using the four points, output "<span class="tex-font-style-tt">Yes</span>". Otherwise, output "<span class="tex-font-style-tt">No</span>".</p><p>You can output the answer in any case. For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">YES</span>" will also be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains four integers $l$, $r$, $d$, $u$ ($1 \le l,r,d,u \le 10$).</p>

## Output

<p>For each test case, if you can draw a square using the four points, output "<span class="tex-font-style-tt">Yes</span>". Otherwise, output "<span class="tex-font-style-tt">No</span>".</p><p>You can output the answer in any case. For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">YES</span>" will also be recognized as positive responses.</p>





```input1|2
2
2 2 2 2
1 2 3 4
```




```output1
Yes
No
```



## Note

<p>On the first test case, the four given points form a square, so the answer is "<span class="tex-font-style-tt">Yes</span>".</p><p>On the second test case, the four given points do not form a square, so the answer is "<span class="tex-font-style-tt">No</span>".</p>
