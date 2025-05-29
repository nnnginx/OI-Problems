## Description

<div><p>  </p><p>You are given a binary string $s$ of length $n$ and a typewriter with two buttons: <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. Initially, your finger is on the button <span class="tex-font-style-tt">0</span>. You can do the following two operations:</p><ol> <li> Press the button your finger is currently on. This will type out the character that is on the button. </li><li> Move your finger to the other button. If your finger is on button <span class="tex-font-style-tt">0</span>, move it to button <span class="tex-font-style-tt">1</span>, and vice versa. </li></ol><p>The <span class="tex-font-style-it">cost</span> of a binary string is defined as the minimum number of operations needed to type the entire string. </p><p>Before typing, you may reverse at most one substring$^{\text{∗}}$ of $s$. More formally, you can choose two indices $1\le l\le r\le n$, and reverse the substring $s_{l\ldots r}$, resulting in the new string $s_1s_2\ldots s_{l-1}s_rs_{r-1}\ldots s_ls_{r+1}\ldots s_n$. </p><p>Your task is to find the minimum possible cost among all strings obtainable by performing at most one substring reversal on $s$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by the deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot 10^5$)&nbsp;— the length of the binary string $s$.</p><p>The second line of each test case contains a binary string $s_1s_2\ldots s_n$ ($s_i = \mathtt{0}$ or $s_i = \mathtt{1}$)&nbsp;— the characters of the binary string $s$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output the minimum cost of string $s$ after performing at most one substring reversal.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2\cdot 10^5$)&nbsp;— the length of the binary string $s$.</p><p>The second line of each test case contains a binary string $s_1s_2\ldots s_n$ ($s_i = \mathtt{0}$ or $s_i = \mathtt{1}$)&nbsp;— the characters of the binary string $s$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, output the minimum cost of string $s$ after performing at most one substring reversal.</p>





```input1|2,3,6,7,10,11
6
3
000
3
111
3
011
3
100
5
10101
19
1101010010011011100
```




```output1
3
4
4
4
8
29
```



## Note

<p>In the first test case, we can choose not to reverse any substrings. We can do operation $1$ three times to type <span class="tex-font-style-tt">000</span>.</p><p>In the second test case, we can choose not to reverse any substrings. We can do operation $2$ to move our finger to button <span class="tex-font-style-tt">1</span>. Then, we do operation $1$ three times to type <span class="tex-font-style-tt">111</span>.</p><p>In the third test case, we can choose not to reverse any substring. We can do operation $1$ to type <span class="tex-font-style-tt">0</span>. Then, we do operation $2$ to move our finger to button <span class="tex-font-style-tt">1</span>. Finally, we do operation $1$ two times to type <span class="tex-font-style-tt">11</span>, resulting in the final string <span class="tex-font-style-tt">011</span> using only $4$ operations.</p><p>In the fourth test case, we can reverse the substring $s_{1\ldots 3}$, resulting in the string <span class="tex-font-style-tt">001</span>. We can do operation $1$ two times to type <span class="tex-font-style-tt">00</span>. Then we do operation $2$ to move our finger to button <span class="tex-font-style-tt">1</span>. Finally, we do operation $1$ once to type <span class="tex-font-style-tt">1</span>, resulting in the final string <span class="tex-font-style-tt">001</span> using only $4$ operations.</p><p>In the fifth test case, we can reverse the substring $s_{2\ldots 3}$, resulting in the string <span class="tex-font-style-tt">11001</span>. The cost of the string is $8$ as we can do the following sequence of operations:</p><ul> <li> Do operation $2$ to move our finger to button <span class="tex-font-style-tt">1</span>. </li><li> Do operation $1$ two times to type <span class="tex-font-style-tt">11</span>. </li><li> Do operation $2$ to move our finger to button <span class="tex-font-style-tt">0</span>. </li><li> Do operation $1$ two times to type <span class="tex-font-style-tt">00</span>. </li><li> Do operation $2$ to move our finger to button <span class="tex-font-style-tt">1</span>. </li><li> Do operation $1$ once to type <span class="tex-font-style-tt">1</span>. </li></ul><p>In the sixth test case, we can reverse the substring $s_{5\ldots 17}$, resulting in the string <span class="tex-font-style-tt">1101</span><span class="tex-font-style-bf">1110110010010</span><span class="tex-font-style-tt">00</span>. It can be proven that the minimum number of operations needed to type the binary string is $29$.</p>
