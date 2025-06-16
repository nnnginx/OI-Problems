## Description

<div><p>Yousef is at the entrance of a long hallway with $n$ doors in a row, numbered from $1$ to $n$. He needs to pass through all the doors from $1$ to $n$ in order of numbering and reach the exit (past door $n$). </p><p>Each door can be open or closed. If a door is open, Yousef passes through it in $1$ second. If the door is closed, Yousef can't pass through it.</p><p>However, Yousef has a special button which he can use <span class="tex-font-style-bf">at most once</span> at any moment. This button makes all closed doors become open for $x$ seconds.</p><p>Your task is to determine if Yousef can pass through all the doors if he can use the button at most once.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>The first line of each test case contains two integers $n, x$ ($1 \le n, x \le 10$) ！ the number of doors and the number of seconds of the button, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, ..., a_n$ ($a_i \in \{0, 1\}$) ！ the state of each door. Open doors are represented by <span class="tex-font-style-tt">'0'</span>, while closed doors are represented by <span class="tex-font-style-tt">'1'</span>.</p><p>It is guaranteed that each test case contains at least one closed door.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if Yousef can reach the exit, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>The first line of each test case contains two integers $n, x$ ($1 \le n, x \le 10$) ！ the number of doors and the number of seconds of the button, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, ..., a_n$ ($a_i \in \{0, 1\}$) ！ the state of each door. Open doors are represented by <span class="tex-font-style-tt">'0'</span>, while closed doors are represented by <span class="tex-font-style-tt">'1'</span>.</p><p>It is guaranteed that each test case contains at least one closed door.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if Yousef can reach the exit, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11,14,15
7
4 2
0 1 1 0
6 3
1 0 1 1 0 0
8 8
1 1 1 0 0 1 1 1
1 2
1
5 1
1 0 1 0 1
7 4
0 0 0 1 1 0 1
10 3
0 1 0 0 1 0 0 1 0 0
```




```output1
YES
NO
YES
YES
NO
YES
NO
```



## Note

<p>In the first test case, the optimal way is as follows: </p><ul> <li> At time $0$, the door is open, so Yousef passes. </li><li> At time $1$, the door is closed, Yousef can use the button now and pass through the door. </li><li> At time $2$, the button's effect is still on, so Yousef can still pass. </li><li> At time $3$, the button's effect has finished, but the door is open. Yousef passes and reaches the exit. </li></ul><p>In the second test case, Yousef has a 3-second button, but he would need at least a 4-second button to reach the exit. Therefore, the answer is <span class="tex-font-style-tt">NO</span>.</p><p>In the third test case, Yousef can turn on the button before starting to move. All the doors will stay open until he reaches the exit.</p>
