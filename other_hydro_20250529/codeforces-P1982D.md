## Description

<div><p>Nikita loves mountains and has finally decided to visit the Berlyand mountain range! The range was so beautiful that Nikita decided to capture it on a map. The map is a table of $n$ rows and $m$ columns, with each cell containing a non-negative integer representing the height of the mountain.</p><p>He also noticed that mountains come in two types:</p><ul> <li> With snowy caps. </li><li> Without snowy caps. </li></ul><p>Nikita is a very pragmatic person. He wants the sum of the heights of the mountains with snowy caps to be equal to the sum of the heights of the mountains without them. He has arranged with the mayor of Berlyand, Polikarp Polikarpovich, to allow him to transform the landscape.</p><p>Nikita can perform transformations on submatrices of size $k \times k$ as follows: he can add an integer constant $c$ to the heights of the mountains within this area, but the type of the mountain remains unchanged. Nikita can choose the constant $c$ independently for each transformation. <span class="tex-font-style-bf">Note that $c$ can be negative</span>.</p><p>Before making the transformations, Nikita asks you to find out if it is possible to achieve equality of the sums, or if it is impossible. It doesn't matter at what cost, even if the mountains turn into canyons and have negative heights.</p><p>If only one type of mountain is represented on the map, then the sum of the heights of the other type of mountain is considered to be zero.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. This is followed by a description of test cases.</p><p>The first line of each test case contains three integers $n, m, k$ ($1 \le n, m \le 500, 1 \le k \le min(n, m)$).</p><p>The next $n$ lines of each test case contain $m$ integers $a_{i j}$ ($0 \le a_{i j} \le 10^{9}$)&nbsp;！ the initial heights of the mountains.</p><p>The next $n$ binary strings of length $m$ for each test case determine the type of mountain, '$0$'&nbsp;！ with snowy caps, '$1$'&nbsp;！ without them.</p><p>It is guaranteed that the sum of $n \cdot m$ for all test cases does not exceed $250\,000$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" without quotes if it is possible to equalize the sums of the mountain heights, otherwise output "<span class="tex-font-style-tt">NO</span>" without quotes. You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of several test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. This is followed by a description of test cases.</p><p>The first line of each test case contains three integers $n, m, k$ ($1 \le n, m \le 500, 1 \le k \le min(n, m)$).</p><p>The next $n$ lines of each test case contain $m$ integers $a_{i j}$ ($0 \le a_{i j} \le 10^{9}$)&nbsp;！ the initial heights of the mountains.</p><p>The next $n$ binary strings of length $m$ for each test case determine the type of mountain, '$0$'&nbsp;！ with snowy caps, '$1$'&nbsp;！ without them.</p><p>It is guaranteed that the sum of $n \cdot m$ for all test cases does not exceed $250\,000$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" without quotes if it is possible to equalize the sums of the mountain heights, otherwise output "<span class="tex-font-style-tt">NO</span>" without quotes. You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,5,6,7,8,18,19,20,21,22,23,24,32,33,34,35,36,37,38,50,51,52,53,54
8
3 3 2
7 11 3
4 2 3
0 1 15
100
010
000
4 4 3
123 413 24 233
123 42 0 216
22 1 1 53
427 763 22 6
0101
1111
1010
0101
3 3 2
2 1 1
1 1 2
1 5 4
010
101
010
3 3 2
2 1 1
1 1 2
1 5 3
010
101
010
3 4 3
46 49 50 1
19 30 23 12
30 25 1 46
1000
0100
0010
5 4 4
39 30 0 17
22 42 30 13
10 44 46 35
12 19 9 39
21 0 45 40
1000
1111
0011
0111
1100
2 2 2
3 4
6 7
00
00
2 2 2
0 0
2 0
01
00
```




```output1
YES
NO
YES
NO
YES
NO
YES
YES
```



## Note

<p>The mountain array from the first test case looks like this:</p><center> <img class="tex-graphics" src="./34724/file/zxgFDqAX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially, the sum of the heights of the mountains with snowy caps is $11 + 3 + 4 + 3 + 0 + 1 + 15 = 37$, and without them is $7 + 2 = 9$.</p><p>To equalize these sums, we can perform two transformations:</p><p>First transformation:</p><center> <img class="tex-graphics" src="./34724/file/kFx6JIbk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that the constant $c$ can be negative.</p><p>After the first transformation, the mountain array looks like this:</p><center> <img class="tex-graphics" src="./34724/file/F4dKSFkG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Second transformation:</p><center> <img class="tex-graphics" src="./34724/file/Wmn59kNR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As a result, the mountain array looks like this:</p><center> <img class="tex-graphics" src="./34724/file/0PG697AE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The sum of the heights of the mountains with snowy caps is $17 + 9 + 9 - 16 - 20 - 19 + 15 = -5$, and without them is $7 - 12 = -5$, thus the answer is <span class="tex-font-style-tt">YES</span>.</p>
