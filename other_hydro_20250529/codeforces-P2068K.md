## Description

<div><p>Ivan, Dmitrii, and Pjotr are celebrating Ivan's birthday at an amusement park with $n$ attractions. The $i$-th attraction operates at minutes $a_i, 2a_i, 3a_i, \dots$ (i.e., every $a_i$ minutes).</p><p>Each minute, the friends can either ride exactly one available attraction <span class="tex-font-style-bf">together</span> or wait. Since the rides are very short, they can board another attraction the next minute. They may ride the attractions in any order.</p><p>They want to experience each ride exactly once before heading off to enjoy the birthday cake. What is the earliest time by which they can finish all $n$ attractions?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 2000$) ！ the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line contains an integer $n$ ($1\le n \le 2000$) ！ the number of attractions. </p><p>The second line contains $n$ integers $a_1,\, a_2,\,\ldots,\, a_n$ ($1 \le a_i \le 10^9$) ！ the values determining when the various attractions operate.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, print the earliest time the three friends can finish all $n$ attractions.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 2000$) ！ the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line contains an integer $n$ ($1\le n \le 2000$) ！ the number of attractions. </p><p>The second line contains $n$ integers $a_1,\, a_2,\,\ldots,\, a_n$ ($1 \le a_i \le 10^9$) ！ the values determining when the various attractions operate.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, print the earliest time the three friends can finish all $n$ attractions.</p>





```input1|2,3,6,7
3
4
1 2 3 4
4
1 1 1 1
6
1 2 1 2 2 2
```




```output1
4
4
8
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, the three friends can ride the $i$-th attraction at the $i$-th minute. Since there are $4$ attractions, they need $4$ minutes to ride them all.</p><p>In the <span class="tex-font-style-bf">third test case</span>, the three friends can ride the attractions in order at minutes $1,\, 2,\, 3,\, 4,\, 6,\, 8$ respectively. Therefore, they can ride all attractions in $8$ minutes. One can show that it is impossible to finish all the attractions earlier.</p>
