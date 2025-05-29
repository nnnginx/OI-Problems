## Description

<div><p>Dmitry has $n$ cubes, numbered from left to right from $1$ to $n$. The cube with index $f$ is his favorite.</p><p>Dmitry threw all the cubes on the table, and the $i$-th cube showed the value $a_i$ ($1 \le a_i \le 100$). After that, he arranged the cubes in non-increasing order of their values, from largest to smallest. If two cubes show the same value, they can go in any order.</p><p>After sorting, Dmitry removed the first $k$ cubes. Then he became interested in whether he removed his favorite cube (note that its position could have changed after sorting).</p><p>For example, if $n=5$, $f=2$, $a = [4, \color{green}3, 3, 2, 3]$ (the favorite cube is highlighted in green), and $k = 2$, the following could have happened:</p><ul> <li> After sorting $a=[4, \color{green}3, 3, 3, 2]$, since the favorite cube ended up in the second position, it will be removed. </li><li> After sorting $a=[4, 3, \color{green}3, 3, 2]$, since the favorite cube ended up in the third position, it will not be removed. </li></ul></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$) ！ the number of test cases. Then follow the descriptions of the test cases.</p><p>The first line of each test case description contains three integers $n$, $f$, and $k$ ($1 \le f, k \le n \le 100$) ！ the number of cubes, the index of Dmitry's favorite cube, and the number of removed cubes, respectively.</p><p>The second line of each test case description contains $n$ integers $a_i$ ($1 \le a_i \le 100$) ！ the values shown on the cubes.</p></div><div class="output-specification"><p>For each test case, output one line ！ "<span class="tex-font-style-tt">YES</span>" if the cube will be removed in all cases, "<span class="tex-font-style-tt">NO</span>" if it will not be removed in any case, "<span class="tex-font-style-tt">MAYBE</span>" if it may be either removed or left.</p><p>You can output the answer in any case. For example, the strings "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">nO</span>", "<span class="tex-font-style-tt">mAyBe</span>" will be accepted as answers.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$) ！ the number of test cases. Then follow the descriptions of the test cases.</p><p>The first line of each test case description contains three integers $n$, $f$, and $k$ ($1 \le f, k \le n \le 100$) ！ the number of cubes, the index of Dmitry's favorite cube, and the number of removed cubes, respectively.</p><p>The second line of each test case description contains $n$ integers $a_i$ ($1 \le a_i \le 100$) ！ the values shown on the cubes.</p>

## Output

<p>For each test case, output one line ！ "<span class="tex-font-style-tt">YES</span>" if the cube will be removed in all cases, "<span class="tex-font-style-tt">NO</span>" if it will not be removed in any case, "<span class="tex-font-style-tt">MAYBE</span>" if it may be either removed or left.</p><p>You can output the answer in any case. For example, the strings "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">nO</span>", "<span class="tex-font-style-tt">mAyBe</span>" will be accepted as answers.</p>





```input1|2,3,6,7,10,11,14,15,18,19,22,23
12
5 2 2
4 3 3 2 3
5 5 3
4 2 1 3 5
5 5 2
5 2 4 1 3
5 5 5
1 2 5 4 3
5 5 4
3 1 2 4 5
5 5 5
4 3 2 1 5
6 5 3
1 2 3 1 2 3
10 1 1
1 1 1 1 1 1 1 1 1 1
1 1 1
42
5 2 3
2 2 1 1 2
2 1 1
2 1
5 3 1
3 3 2 3 2
```




```output1
MAYBE
YES
NO
YES
YES
YES
MAYBE
MAYBE
YES
YES
YES
NO
```


