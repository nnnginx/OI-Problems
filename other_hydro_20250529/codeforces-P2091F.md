## Description

<div><p>The visitors of the IT Campus "NEIMARK" are not only strong programmers but also physically robust individuals! Some practice swimming, some rowing, and some rock climbing!</p><p>Master Igor is a prominent figure in the local rock climbing community. One day, he went on a mountain hike to ascend one of the peaks. As an experienced climber, Igor decided not to follow the established trails but to use his skills to climb strictly vertically.</p><p>Igor found a rectangular vertical section of the mountain and mentally divided it into $n$ horizontal levels. He then split each level into $m$ segments using vertical partitions. Upon inspecting these segments, Igor discovered convenient protrusions that can be grasped (hereafter referred to as <span class="tex-font-style-it">holds</span>). Thus, the selected part of the mountain can be represented as an $n \times m$ rectangle, with some cells containing holds.</p><p>Being an experienced programmer, Igor decided to count the number of valid <span class="tex-font-style-it">routes</span>. A route is defined as a sequence of <span class="tex-font-style-bf">distinct</span> holds. A route is considered valid if the following conditions are satisfied: </p><ul> <li> The first hold in the route is located on the very bottom level (row $n$); </li><li> The last hold in the route is located on the very top level (row $1$); </li><li> Each subsequent hold is not lower than the previous one; </li><li> At least one hold is used on each level (i.e., in every row of the rectangle); </li><li> At most two holds are used on each level (since Igor has only two hands); </li><li> Igor can reach from the current hold to the next one if the distance between the centers of the corresponding sections does not exceed Igor's arm span. </li></ul><p>Igor's arm span is $d$, which means he can move from one hold to another if the <span class="tex-font-style-bf">Euclidean distance</span> between the centers of the corresponding segments does not exceed $d$. The distance between sections ($i_1, j_1$) and ($i_2, j_2$) is given by $\sqrt{(i_1 - i_2) ^ 2 + (j_1 - j_2) ^ 2}$.</p><p>Calculate the number of different valid routes. Two routes are considered different if they differ in the list of holds used or in the order in which these holds are visited.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^3$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, $d$ ($2 \leq n \leq 2000$, $1 \leq m, d \leq 2000$).</p><p>Each of the following $n$ lines contains $m$ characters&nbsp;¡ª the description of the corresponding level of the mountain. The symbol '#' represents an empty section, and the symbol 'X' represents a section with a hold. The levels are described from top to bottom.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $4 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output the number of different routes modulo $998244353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^3$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, $d$ ($2 \leq n \leq 2000$, $1 \leq m, d \leq 2000$).</p><p>Each of the following $n$ lines contains $m$ characters&nbsp;¡ª the description of the corresponding level of the mountain. The symbol '#' represents an empty section, and the symbol 'X' represents a section with a hold. The levels are described from top to bottom.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $4 \cdot 10^6$.</p>

## Output

<p>For each test case, output the number of different routes modulo $998244353$.</p>





```input1|2,3,4,5,10,11,12,13
3
3 4 1
XX#X
#XX#
#X#X
3 4 2
XX#X
#XX#
#X#X
3 1 3
X
X
#
```




```output1
2
60
0
```



## Note

<p>Possible routes in the first case: </p><center> <img class="tex-graphics" src="./37198/file/go0K6Eh6.png" style="zoom: 75.0%;max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, Igor's arm span has become larger, so new routes are available to him, for example this one: </p><center> <img class="tex-graphics" src="./37198/file/FD8rq3py.png" style="zoom: 75.0%;max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, there are no holds on the lower level, so there are no correct routes.</p>
