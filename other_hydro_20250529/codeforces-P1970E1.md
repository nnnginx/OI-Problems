## Description

<div><p>Harry Potter is hiking in the Alps surrounding Lake Geneva. In this area there are $m$ cabins, numbered 1 to $m$. Each cabin is connected, with one or more trails, to a central meeting point next to the lake. Each trail is either <span class="tex-font-style-underline">short</span> or <span class="tex-font-style-underline">long</span>. Cabin $i$ is connected with $s_i$ short trails and $l_i$ long trails to the lake.</p><p>Each day, Harry walks a trail from the cabin where he currently is to Lake Geneva, and then from there he walks a trail to any of the $m$ cabins (including the one he started in). However, as he has to finish the hike in a day, at least one of the two trails has to be short.</p><p>How many possible combinations of trails can Harry take if he starts in cabin 1 and walks for $n$ days?</p><p>Give the answer modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains the integers $m$ and $n$.</p><p>The second line contains $m$ integers, $s_1, \dots, s_m$, where $s_i$ is the number of short trails between cabin $i$ and Lake Geneva.</p><p>The third and last line contains $m$ integers, $l_1, \dots, l_m$, where $l_i$ is the number of long trails between cabin $i$ and Lake Geneva.</p><p>We have the following constraints:</p><p>$0 \le s_i, l_i \le 10^3$.</p><p>$1 \le m \le 10^2$.</p><p>$1 \le n \le 10^3$.</p></div><div class="output-specification"><p>The number of possible combinations of trails, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains the integers $m$ and $n$.</p><p>The second line contains $m$ integers, $s_1, \dots, s_m$, where $s_i$ is the number of short trails between cabin $i$ and Lake Geneva.</p><p>The third and last line contains $m$ integers, $l_1, \dots, l_m$, where $l_i$ is the number of long trails between cabin $i$ and Lake Geneva.</p><p>We have the following constraints:</p><p>$0 \le s_i, l_i \le 10^3$.</p><p>$1 \le m \le 10^2$.</p><p>$1 \le n \le 10^3$.</p>

## Output

<p>The number of possible combinations of trails, modulo $10^9 + 7$.</p>





```input1|
3 2
1 0 1
0 1 1
```




```output1
18
```


