## Description

<div><p>DLS and JLS are bored with a Math lesson. In order to entertain themselves, DLS took a sheet of paper and drew $n$ distinct lines, given by equations $y = x + p_i$ for some distinct $p_1, p_2, \ldots, p_n$.</p><p>Then JLS drew on the same paper sheet $m$ distinct lines given by equations $y = -x + q_i$ for some distinct $q_1, q_2, \ldots, q_m$.</p><p>DLS and JLS are interested in counting how many line pairs have <span class="tex-font-style-bf">integer</span> intersection points, i.e. points with both coordinates that are integers. Unfortunately, the lesson will end up soon, so DLS and JLS are asking for your help.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$), the number of test cases in the input. Then follow the test case descriptions.</p><p>The first line of a test case contains an integer $n$ ($1 \le n \le 10^5$), the number of lines drawn by DLS.</p><p>The second line of a test case contains $n$ distinct integers $p_i$ ($0 \le p_i \le 10^9$) describing the lines drawn by DLS. The integer $p_i$ describes a line given by the equation $y = x + p_i$.</p><p>The third line of a test case contains an integer $m$ ($1 \le m \le 10^5$), the number of lines drawn by JLS.</p><p>The fourth line of a test case contains $m$ distinct integers $q_i$ ($0 \le q_i \le 10^9$) describing the lines drawn by JLS. The integer $q_i$ describes a line given by the equation $y = -x + q_i$.</p><p>The sum of the values of $n$ over all test cases in the input does not exceed $10^5$. Similarly, the sum of the values of $m$ over all test cases in the input does not exceed $10^5$.</p><p><span class="tex-font-style-bf">In hacks</span> it is allowed to use only one test case in the input, so $t=1$ should be satisfied.</p></div><div class="output-specification"><p>For each test case in the input print a single integer&nbsp;�� the number of line pairs with integer intersection points. </p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$), the number of test cases in the input. Then follow the test case descriptions.</p><p>The first line of a test case contains an integer $n$ ($1 \le n \le 10^5$), the number of lines drawn by DLS.</p><p>The second line of a test case contains $n$ distinct integers $p_i$ ($0 \le p_i \le 10^9$) describing the lines drawn by DLS. The integer $p_i$ describes a line given by the equation $y = x + p_i$.</p><p>The third line of a test case contains an integer $m$ ($1 \le m \le 10^5$), the number of lines drawn by JLS.</p><p>The fourth line of a test case contains $m$ distinct integers $q_i$ ($0 \le q_i \le 10^9$) describing the lines drawn by JLS. The integer $q_i$ describes a line given by the equation $y = -x + q_i$.</p><p>The sum of the values of $n$ over all test cases in the input does not exceed $10^5$. Similarly, the sum of the values of $m$ over all test cases in the input does not exceed $10^5$.</p><p><span class="tex-font-style-bf">In hacks</span> it is allowed to use only one test case in the input, so $t=1$ should be satisfied.</p>

## Output

<p>For each test case in the input print a single integer&nbsp;�� the number of line pairs with integer intersection points. </p>

## Samples

```input1
3
3
1 3 2
2
0 3
1
1
1
1
1
2
1
1
```

```output1
3
1
0
```




## Note

<p>The picture shows the lines from the first test case of the example. Black circles denote intersection points with integer coordinates.</p><center> <img class="tex-graphics" height="453px" src="./30601/file/4se40BfI.png" style="max-width: 100.0%;max-height: 100.0%;" width="453px"> </center>
