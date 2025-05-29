## Description

<div><p>  </p><p><span class="tex-font-style-it">This is an interactive problem.</span> </p><p>The pink soldiers hid from you $n$ ($3 \le n \le 1500$) <span class="tex-font-style-bf">fixed</span> points $(x_1,y_1), (x_2,y_2), \ldots, (x_n,y_n)$, <span class="tex-font-style-bf">whose coordinates are not given to you</span>. Also, it is known that no two points have the same coordinates, and no three points are <a href="https://en.wikipedia.org/wiki/Collinearity">collinear</a>.</p><p>You can ask the Frontman about three <span class="tex-font-style-bf">distinct</span> indices $i$, $j$, $k$. Then, he will draw a triangle with points $(x_i,y_i)$, $(x_j,y_j)$, $(x_k,y_k)$, and respond with the following:</p><ul> <li> If at least one of the hidden points lies inside the triangle, then the Frontman gives you the index of one such point. Do note that if there are multiple such points, <span class="tex-font-style-bf">the Frontman can arbitrarily select one of them</span>. </li><li> Otherwise, the Frontman responds with $0$. </li></ul><center> <img class="tex-graphics" src="./36014/file/2BLedE9G.png" style="max-width: 100.0%;max-height: 100.0%;">  <span class="tex-font-size-small">Your objective in this problem is to find a triangle not containing any other hidden point, such as the blue one in the diagram.</span> </center><p>Using at most $\mathbf{75}$ queries, you must find any triangle formed by three of the points, <span class="tex-font-style-bf">not containing</span> any other hidden point inside.</p><p>Do note that the Frontman may be <span class="tex-font-style-bf">adaptive</span> while choosing the point to give you. In other words, the choice of the point can be determined by various factors including but not limited to the orientation of points and the previous queries. However, note that <span class="tex-font-style-bf">the sequence of points will never be altered</span>.</p><p>Hacks are disabled for this problem. Your solution will be judged on exactly $\mathbf{35}$ input files, including the example input.</p></div><div><h2>Interaction</h2><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 20$). The description of the test cases follows. </p><p>The first line of each test case contains one positive integer $n$&nbsp;— the number of points ($3 \le n \le 1500$).</p><p>Afterwards, you can output the following on a separate line to ask a query:</p><ul> <li> "<span class="tex-font-style-tt">? i j k</span>" ($1 \le i,j,k \le n$, $i \ne j$, $i \ne k$, $j \ne k$): Ask about the triangle formed by $(x_i,y_i)$, $(x_j,y_j)$, $(x_k,y_k)$. </li></ul><p>Then, the interactor responds with one integer on a new line:</p><ul> <li> If your query is invalid or the number of queries has exceeded $\mathbf{75}$, then the interactor responds with $-1$; </li><li> If there exists an index $p$ ($1 \le p \le n$) such that the point $(x_p,y_p)$ is inside the triangle, then <span class="tex-font-style-bf">any such index</span> $p$ is given; </li><li> Otherwise, the interactor responds with $0$. </li></ul><p>If you want to print an answer, you can output the following on a separate line:</p><ul> <li> "<span class="tex-font-style-tt">! i j k</span>" ($1 \le i,j,k \le n$, $i \ne j$, $i \ne k$, $j \ne k$): The triangle formed by $(x_i,y_i)$, $(x_j,y_j)$, $(x_k,y_k)$ contains no other hidden point. </li></ul><p>Then, the following interaction happens:</p><ul><li> If the answer is invalid or the triangle contains another hidden point, the interactor responds with $-1$; </li><li> If the answer is correct and there are more test cases to solve, you are given the value of $n$ for the next test case; </li><li> Otherwise, it means that all test cases are solved correctly, and your program may terminate gracefully. </li></ul><p>Do note that printing the answer does <span class="tex-font-style-bf">not</span> count towards the number of queries made.</p><p>Do note that the interactor may be <span class="tex-font-style-bf">adaptive</span> while choosing the point to give you. In other words, the choice of the point can be determined by various factors including but not limited to the orientation of points and the previous queries. However, note that <span class="tex-font-style-bf">the sequence of points will never be altered</span>.</p><p>After printing each query do not forget to output the end of line and flush$^{\text{∗}}$ the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict.</p><p>If, at any interaction step, you read $-1$ instead of valid data, your solution must exit immediately. This means that your solution will receive <span class="tex-font-style-tt">Wrong answer</span> because of an invalid query or any other mistake. Failing to exit can result in an arbitrary verdict because your solution will continue to read from a closed stream. </p><p><span><span class="tex-font-style-bf">Hacks</span></span></p><p>Hacks are disabled for this problem. Your solution will be judged on exactly $\mathbf{35}$ input files, including the example input.</p><div class="statement-footnote"><p>$^{\text{∗}}$To flush, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">sys.stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul></div></div>





```input1
2
6

5

4

0

3
```




```output1
? 1 2 3

? 1 5 3

? 2 5 6

! 2 5 6

! 1 2 3
```



## Note

<p>In the first test case, the points are $(3,0),(0,3),(5,2),(3,1),(2,2),(4,4)$.</p><p>The triangles corresponding to the three queries are as follows.</p><center> <img class="tex-graphics" src="./36014/file/otSCMFV4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You can see that the triangle formed by $(0,3)$, $(2,2)$, $(4,4)$ does not contain any other hidden point inside. Therefore, it is a valid answer.</p><p>Do note that the interaction example only shows a valid interaction, and <span class="tex-font-style-bf">not necessarily the actual response</span>. For example, it is possible that the Frontman responds with $4$ when you query "<span class="tex-font-style-tt">? 1 2 3</span>". However, as the Frontman does not alter the sequence of points, he never responds with $6$ for the same query.</p><p>In the second test case, there are only $3$ points. Therefore, we know that the unique triangle formed by the points does not contain any other hidden point inside.</p>
