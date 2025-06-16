## Description

<div><p>There are very long classes in the T-Generation. In one day, you need to have time to analyze the training and thematic contests, give a lecture with new material, and, if possible, also hold a mini-seminar. Therefore, there is a break where students can go to drink coffee and chat with each other.</p><p>There are a total of $n+2$ coffee machines located in sequentially arranged rooms along a long corridor. The coffee machines are numbered from $0$ to $n+1$, and immediately after the break starts, there are $a_i$ students gathered around the $i$-th coffee machine.</p><p>The students are talking too loudly among themselves, and the teachers need to make a very important announcement. Therefore, they want to gather the maximum number of students around some single coffee machine. The teachers are too lazy to run around the corridors and gather the students, so they came up with a more sophisticated way to manipulate them:</p><ul> <li> At any moment, the teachers can choose room $i$ ($1 \le i \le n$) and turn off the lights there; </li><li> If there were $x$ students in that room, then after turning off the lights, $\lfloor \frac12 x \rfloor$ students will go to room $(i-1)$, and $\lfloor \frac12 x \rfloor$ other students will go to room $(i+1)$. </li><li> If $x$ was odd, then one student remains in the same room. </li><li> After that, the lights in room $i$ are turned back on. </li></ul><p>The teachers have not yet decided where they will gather the students, so for each $i$ from $1$ to $n$, you should determine what is the maximum number of students that can be gathered around the $i$-th coffee machine.</p><p>The teachers can turn off the lights in any rooms at their discretion, in any order, possibly turning off the lights in the same room multiple times.</p><p>Note that the values of $a_0$ and $a_{n+1}$ do not affect the answer to the problem, so their values will not be given to you.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;�� the number of test cases.</p><p>In the first line of each test case, there is an integer $n$ ($1 \le n \le 10^6$).</p><p>In the second line of each test case, there are integers $a_1, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;�� the number of students around coffee machines numbered $1, 2, \ldots, n$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $b_1, \ldots, b_n$, where $b_i$ is the maximum number of students that can be around coffee machines number $i$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;�� the number of test cases.</p><p>In the first line of each test case, there is an integer $n$ ($1 \le n \le 10^6$).</p><p>In the second line of each test case, there are integers $a_1, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;�� the number of students around coffee machines numbered $1, 2, \ldots, n$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output $n$ integers $b_1, \ldots, b_n$, where $b_i$ is the maximum number of students that can be around coffee machines number $i$.</p>





```input1|2,3,6,7
3
2
8 0
5
2 2 2 2 2
5
0 0 9 0 0
```




```output1
8 4 
4 5 4 5 4 
4 6 9 6 4
```



## Note

<p>Let's analyze the first test case:</p><ul> <li> To maximize the number of students at the $1$-st coffee machine, all that needs to be done is nothing. </li><li> To maximize the number of students at the $2$-nd coffee machine, it is sufficient to turn off the lights in the $1$-st room once. </li></ul>
