## Description

<div><p>As meticulous Gerald sets the table and caring Alexander sends the postcards, Sergey makes snowmen. Each showman should consist of three snowballs: a big one, a medium one and a small one. Sergey's twins help him: they've already made <span class="tex-span"><i>n</i></span> snowballs with radii equal to <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>r</i><sub class="lower-index"><i>n</i></sub></span>. To make a snowman, one needs any three snowballs whose radii are pairwise different. For example, the balls with radii <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> can be used to make a snowman but <span class="tex-span">2</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> or <span class="tex-span">2</span>, <span class="tex-span">2</span>, <span class="tex-span">2</span> cannot. Help Sergey and his twins to determine what <span class="tex-font-style-bf">maximum</span> number of snowmen they can make from those snowballs.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of snowballs. The next line contains <span class="tex-span"><i>n</i></span> integers — the balls' radii <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The balls' radii can coincide.</p></div><div class="output-specification"><p>Print on the first line a single number <span class="tex-span"><i>k</i></span> — the maximum number of the snowmen. Next <span class="tex-span"><i>k</i></span> lines should contain the snowmen's descriptions. The description of each snowman should consist of three space-separated numbers — the big ball's radius, the medium ball's radius and the small ball's radius. It is allowed to print the snowmen in any order. If there are several solutions, print any of them.</p></div>


## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of snowballs. The next line contains <span class="tex-span"><i>n</i></span> integers — the balls' radii <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The balls' radii can coincide.</p>


## Output

<p>Print on the first line a single number <span class="tex-span"><i>k</i></span> — the maximum number of the snowmen. Next <span class="tex-span"><i>k</i></span> lines should contain the snowmen's descriptions. The description of each snowman should consist of three space-separated numbers — the big ball's radius, the medium ball's radius and the small ball's radius. It is allowed to print the snowmen in any order. If there are several solutions, print any of them.</p>


## Samples

```input1
7
1 2 3 4 5 6 7

```

```output1
2
3 2 1
6 5 4

```






```input2
3
2 2 3

```

```output2
0

```



