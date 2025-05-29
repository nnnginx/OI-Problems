## Description

<div><p>As soon as Dasha Purova crossed the border of France, the villain Markaron kidnapped her and placed her in a prison under his large castle. Fortunately, the wonderful Lady Bug, upon hearing the news about Dasha, immediately ran to save her in Markaron's castle. However, to get there, she needs to crack a complex password.</p><p>The password consists of two bit strings $a$ and $b$, each of which has a length of $n$. In one operation, Lady Bug can choose any index $2 \le i \le n$ and perform one of the following actions: </p><ol> <li> swap($a_i$, $b_{i-1}$) (swap the values of $a_i$ and $b_{i-1}$), or </li><li> swap($b_i$, $a_{i-1}$) (swap the values of $b_i$ and $a_{i-1}$). </li></ol><p>Lady Bug can perform any number of operations. The password is considered cracked if she can ensure that the first string consists only of zeros. Help her understand whether or not she will be able to save the unfortunate Dasha.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) ！ the length of the bit strings of the password. </p><p>The next two lines contain the bit strings of length $n$, $a$ and $b$, which represent the password. Each of the strings contains only the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">'1'</span>. </p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if Lady Bug can crack the password after any number of operations; otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) ！ the length of the bit strings of the password. </p><p>The next two lines contain the bit strings of length $n$, $a$ and $b$, which represent the password. Each of the strings contains only the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">'1'</span>. </p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if Lady Bug can crack the password after any number of operations; otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,3,4,8,9,10
4
3
000
000
6
010001
010111
5
10000
01010
2
11
00
```




```output1
YES
YES
NO
YES
```



## Note

<p>In the first test case, the string $a$ immediately consists only of zeros.</p><p>In the second test case, a possible sequence of operations is:</p><ol> <li><p>swap$(a_2, \ b_{1})$</p><p>$\mathtt{0{\color{red}{1}}0001}$</p><p>$\mathtt{{\color{red}{0}}10111}$</p></li><li><p>swap$(b_5, \ a_{4})$</p><p>$\mathtt{000{\color{red}{0}}01}$</p><p>$\mathtt{1101{\color{red}{1}}1}$</p></li><li><p>swap$(a_4, \ b_{3})$</p><p>$\mathtt{000{\color{red}{1}}01}$</p><p>$\mathtt{11{\color{red}{0}}101}$</p></li><li><p>swap$(a_5, \ b_{4})$</p><p>$\mathtt{00000{\color{red}{1}}}$</p><p>$\mathtt{1111{\color{red}{0}}1}$</p></li></ol>
