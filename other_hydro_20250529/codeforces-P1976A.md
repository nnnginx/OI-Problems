## Description

<div><p>Monocarp is working on his new site, and the current challenge is to make the users pick strong passwords.</p><p>Monocarp decided that strong passwords should satisfy the following conditions: </p><ul> <li> password should consist only of lowercase Latin letters and digits; </li><li> there should be no digit that comes after a letter (so, after each letter, there is either another letter or the string ends); </li><li> all digits should be sorted in the non-decreasing order; </li><li> all letters should be sorted in the non-decreasing order. </li></ul><p>Note that it's allowed for the password to have only letters or only digits.</p><p>Monocarp managed to implement the first condition, but he struggles with the remaining ones. Can you help him to verify the passwords?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 20$)&nbsp;！ the length of the password.</p><p>The second line contains a string, consisting of exactly $n$ characters. Each character is either a lowercase Latin letter or a digit.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if the given password is strong and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 20$)&nbsp;！ the length of the password.</p><p>The second line contains a string, consisting of exactly $n$ characters. Each character is either a lowercase Latin letter or a digit.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if the given password is strong and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1|2,3,6,7,10,11
5
4
12ac
5
123wa
9
allllmost
5
ac123
6
011679
```




```output1
YES
NO
YES
NO
YES
```



## Note

<p>In the second testcase, the letters are not sorted in the non-decreasing order.</p><p>In the fourth testcase, there is a digit that comes after a letter&nbsp;！ digit '1' after a letter 'c'.</p>
