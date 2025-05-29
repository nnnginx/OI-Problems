## Description

<div><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><span class="tex-font-style-it">The Frontman greets you to this final round of the survival game.</span></td></tr></tbody></table> </center><p>There is a regular polygon with $n$ sides ($n \ge 3$). The vertices are indexed as $1,2,\ldots,n$ in clockwise order. On each vertex $i$, the pink soldiers have written a positive integer $a_i$. With this regular polygon, you will play a game defined as follows.</p><p>Initially, your score is $0$. Then, you perform the following operation any number of times to increase your score.</p><ul> <li> Select $3$ different vertices $i$, $j$, $k$ that you <span class="tex-font-style-bf">have not chosen</span> before, and draw the triangle formed by the three vertices. <ul> <li> Then, your score increases by $a_i \cdot a_j \cdot a_k$. </li><li> However, you <span class="tex-font-style-bf">can not perform this operation</span> if the triangle shares a positive common area with any of the triangles drawn previously. </li></ul> </li></ul><center> <img class="tex-graphics" src="./36012/file/RMOLl22S.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">An example of a state after two operations is on the left. The state on the right <span class="tex-font-style-bf">is impossible</span> as the two triangles share a positive common area.</span> </center><p>Your objective is to maximize the score. Please find the maximum score you can get from this game.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$&nbsp;！ the number of vertices ($3 \le n \le 400$).</p><p>The second line of each test case contains $a_1,a_2,\ldots,a_n$&nbsp;！ the integers written on vertices ($1 \le a_i \le 1000$).</p><p>It is guaranteed that the sum of $n^3$ over all test cases does not exceed $400^3$.</p></div><div class="output-specification"><p>For each test case, output the maximum score you can get on a separate line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$&nbsp;！ the number of vertices ($3 \le n \le 400$).</p><p>The second line of each test case contains $a_1,a_2,\ldots,a_n$&nbsp;！ the integers written on vertices ($1 \le a_i \le 1000$).</p><p>It is guaranteed that the sum of $n^3$ over all test cases does not exceed $400^3$.</p>

## Output

<p>For each test case, output the maximum score you can get on a separate line.</p>





```input1|2,3,6,7,10,11
6
3
1 2 3
4
2 1 3 4
6
2 1 2 1 1 1
6
1 2 1 3 1 5
9
9 9 8 2 4 4 3 5 3
9
9 9 3 2 4 4 8 5 3
```




```output1
6
24
5
30
732
696
```



## Note

<p>On the first test case, you can draw only one triangle. The maximum score $6$ is found by drawing the triangle with $i=1$, $j=2$, $k=3$.</p><p>On the second test case, you can draw only one triangle. The maximum score $24$ is found by drawing the triangle with $i=1$, $j=3$, $k=4$.</p><p>On the third test case, you can draw two triangles. There is a series of two operations that leads to the score $5$, which is the maximum.</p><p>On the fourth test case, you can draw two triangles. However, drawing two triangles leads to a score of either $6+5=11$, $15+2=17$, or $10+3=13$. The maximum score $30$ is found by drawing <span class="tex-font-style-bf">only one</span> triangle with $i=2$, $j=4$, $k=6$.</p><p>On the fifth test case, you can draw three triangles. The maximum score $732$ is found by drawing three triangles as follows.</p><center> <img class="tex-graphics" src="./36012/file/0ZnCfAiR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
