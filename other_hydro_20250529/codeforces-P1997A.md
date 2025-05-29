## Description

<div><p>Monocarp's current password on Codeforces is a string $s$, consisting of lowercase Latin letters. Monocarp thinks that his current password is too weak, so he wants to <span class="tex-font-style-bf">insert exactly one lowercase Latin letter</span> into the password to make it stronger. Monocarp can choose any letter and insert it anywhere, even before the first character or after the last character.</p><p>Monocarp thinks that the password's strength is proportional to the time it takes him to type the password. The time it takes to type the password is calculated as follows:</p><ul> <li> the time to type the first character is $2$ seconds; </li><li> for each character other than the first, the time it takes to type it is $1$ second if it is the same as the previous character, or $2$ seconds otherwise. </li></ul><p>For example, the time it takes to type the password <span class="tex-font-style-tt">abacaba</span> is $14$; the time it takes to type the password <span class="tex-font-style-tt">a</span> is $2$; the time it takes to type the password <span class="tex-font-style-tt">aaabacc</span> is $11$.</p><p>You have to help Monocarp ！ insert a lowercase Latin letter into his password so that the resulting password takes the maximum possible amount of time to type.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 10$), consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, print one line containing the new password ！ a string which can be obtained from $s$ by inserting one lowercase Latin letter. The string you print should have the maximum possible required time to type it. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 10$), consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, print one line containing the new password ！ a string which can be obtained from $s$ by inserting one lowercase Latin letter. The string you print should have the maximum possible required time to type it. If there are multiple answers, print any of them.</p>





```input1|2,4
4
a
aaa
abb
password
```




```output1
wa
aada
abcb
pastsword
```


