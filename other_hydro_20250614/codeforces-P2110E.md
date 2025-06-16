## Description

<div><p>In 2077, the robots that took over the world realized that human music wasn't that great, so they started composing their own.</p><p>To write music, the robots have a special musical instrument capable of producing $n$ different sounds. Each sound is characterized by its volume and pitch. A sequence of sounds is called music. Music is considered <span class="tex-font-style-tt">beautiful</span> if any two consecutive sounds differ either only in volume or only in pitch. Music is considered <span class="tex-font-style-tt">boring</span> if the volume or pitch of any three consecutive sounds is the same.</p><p>You want to compose <span class="tex-font-style-tt">beautiful</span>, <span class="tex-font-style-bf">non</span>-<span class="tex-font-style-tt">boring</span> music that contains each sound produced by your musical instrument exactly once.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>In the first line of each test case, there is a number $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of sounds that the musical instrument can produce.</p><p>Next, there are $n$ lines, where the $i$-th line contains a pair of numbers $v_i, p_i$ ($1 \le v_i,\space p_i \le 10^9$)&nbsp;！ the volume and pitch of the $i$-th sound, respectively. It is guaranteed that among all $n$ sounds, there are no duplicates, meaning for any $i \neq j$, at least one of the conditions $v_i \neq v_j$ or $p_i \neq p_j$ holds.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if it is possible to compose such music, output "<span class="tex-font-style-tt">YES</span>", and on the next line, output $n$ numbers&nbsp;！ the indices of the sounds in the order that forms beautiful non-boring music. Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>In the first line of each test case, there is a number $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of sounds that the musical instrument can produce.</p><p>Next, there are $n$ lines, where the $i$-th line contains a pair of numbers $v_i, p_i$ ($1 \le v_i,\space p_i \le 10^9$)&nbsp;！ the volume and pitch of the $i$-th sound, respectively. It is guaranteed that among all $n$ sounds, there are no duplicates, meaning for any $i \neq j$, at least one of the conditions $v_i \neq v_j$ or $p_i \neq p_j$ holds.</p><p>The sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, if it is possible to compose such music, output "<span class="tex-font-style-tt">YES</span>", and on the next line, output $n$ numbers&nbsp;！ the indices of the sounds in the order that forms beautiful non-boring music. Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,3,4,5,6,11,12,19,20,21,22,23,24,25,26
5
4
179 239
179 179
239 179
239 239
3
1 1
2 1
3 1
1
5 7
5
1 1
1 2
2 1
2 2
99 99
7
1 1
1 3
2 1
2 2
3 1
3 2
3 3
```




```output1
YES
4 3 2 1 
NO
YES
1 
NO
YES
3 4 6 7 2 1 5
```



## Note

<p>In the first test case, the music $(239,239)-(239,179)-(179,179)-(179,239)$ is suitable, contains all sounds, and all consecutive sounds differ either only in volume or only in pitch.</p><p>In the second test case, it can be shown that there is no suitable music with the given sounds.</p>
