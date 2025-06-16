## Description

<div><p>A new semester is about to begin, and it is necessary to create a schedule for the first day. There are a total of $n$ groups and $m$ classrooms in the faculty. It is also known that each group has exactly $6$ classes on the first day, and the $k$-th class of each group takes place at the same time. Each class must be held in a classroom, and at the same time, there cannot be classes for more than one group in the same classroom.</p><p>Each classroom has its own index (at least three digits), and all digits of this index, except for the last two, indicate the floor on which the classroom is located. For example, classroom $479$ is located on the $4$-th floor, while classroom $31415$ is on the $314$-th floor. Between floors, one can move by stairs; for any floor $x &gt; 1$, one can either go down to floor $x - 1$ or go up to floor $x + 1$; from the first floor, one can only go up to the second; from the floor $10^7$ (which is the last one), it is possible to go only to the floor $9999999$.</p><p>The faculty's dean's office has decided to create the schedule in such a way that students move as much as possible between floors, meaning that <span class="tex-font-style-bf">the total number of movements between floors across all groups should be maximized</span>. When the students move from one floor to another floor, they take the shortest path.</p><p>For example, if there are $n = 2$ groups and $m = 4$ classrooms $[479, 290, 478, 293]$, the schedule can be arranged as follows:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Class No.</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Group 1</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Group 2</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$290$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$293$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$478$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$479$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$293$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$290$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$479$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$478$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$293$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$290$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$479$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$478$</td></tr></tbody></table> </center><p>In such a schedule, the groups will move between the $2$nd and $4$th floors each time, resulting in a total of $20$ movements between floors.</p><p>Help the dean's office create any suitable schedule!</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{3}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 10^{5}$)&nbsp;！ the number of groups and the number of available classrooms.</p><p>The second line of each test case contains $m$ integers $a_{i}$ ($100 \le a_{i} &lt; 10^{9}$)&nbsp;！ the indices of the available classrooms.</p><p>Additional constraints on the input:</p><ul> <li> the numbers of all classrooms are pairwise distinct; </li><li> the sum of $m$ across all test cases does not exceed $10^{5}$. </li></ul></div><div class="output-specification"><p>For each test case, output $n$ lines, where the $i$-th line should contain $6$ integers&nbsp;！ the indices of the classrooms where the classes for the $i$-th group will be held.</p><p>Each classroom must be occupied by at most one group during the $k$-th class.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{3}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 10^{5}$)&nbsp;！ the number of groups and the number of available classrooms.</p><p>The second line of each test case contains $m$ integers $a_{i}$ ($100 \le a_{i} &lt; 10^{9}$)&nbsp;！ the indices of the available classrooms.</p><p>Additional constraints on the input:</p><ul> <li> the numbers of all classrooms are pairwise distinct; </li><li> the sum of $m$ across all test cases does not exceed $10^{5}$. </li></ul>

## Output

<p>For each test case, output $n$ lines, where the $i$-th line should contain $6$ integers&nbsp;！ the indices of the classrooms where the classes for the $i$-th group will be held.</p><p>Each classroom must be occupied by at most one group during the $k$-th class.</p>





```input1|2,3,6,7
3
2 4
479 290 478 293
1 1
31415
6 10
479 385 290 293 384 383 297 478 291 382
```




```output1
290 478 293 479 293 479
293 479 290 478 290 478
31415 31415 31415 31415 31415 31415
479 290 479 290 479 290
290 479 290 479 290 479
293 478 293 478 293 478
297 385 297 385 297 385
478 293 478 293 478 293
291 384 291 384 291 384
```



## Note

<p>In the third test case, the maximum number of moves between classrooms is $50$.</p>
