## Description

<div><p>You're a linguist studying a mysterious ancient language. You know that </p><ol> <li> Its words consist only of the first $c$ letters of the Latin alphabet. </li><li> Each word has a <span class="tex-font-style-it">case</span> which can be unambiguously determined by its last letter (different letters correspond to different cases). For example, words <span class="tex-font-style-tt">"ABACABA"</span> and <span class="tex-font-style-tt">"ABA"</span> (if they exist) have the same case in this language because they both have the same ending <span class="tex-font-style-tt">'A'</span>, whereas <span class="tex-font-style-tt">"ALICE"</span> and <span class="tex-font-style-tt">"BOB"</span> have different cases. If the language does not have a case corresponding to some letter, it means that the word cannot end with this letter. </li><li> The length of each word is $k$ or less. </li></ol><p>You have a single text written in this language. Unfortunately, as the language is really ancient, spaces between words are missing and all letters are uppercase. You wonder what is the minimum number of cases the language can have. Can you find this out?</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;！ the number of test cases. It is followed by descriptions of the test cases.</p><p>The first line of each test case contains three integers $n$, $c$, $k$ ($1 \le k \le n \le 2^{18}$, $1 \le c \le 18$)&nbsp;！ the length of the text, the number of letters in the language, and the maximum length of the word.</p><p>The second line contains a string of $n$ characters&nbsp;！ the text itself. Each character is one of the first $c$ uppercase letters of the Latin alphabet.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2^{18}$ and the sum of $2^c$ over all test cases does not exceed $2^{18}$.</p></div><div class="output-specification"><p>For each test case, output a single line consisting of a single integer&nbsp;！ the minimum number of cases in the language.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;！ the number of test cases. It is followed by descriptions of the test cases.</p><p>The first line of each test case contains three integers $n$, $c$, $k$ ($1 \le k \le n \le 2^{18}$, $1 \le c \le 18$)&nbsp;！ the length of the text, the number of letters in the language, and the maximum length of the word.</p><p>The second line contains a string of $n$ characters&nbsp;！ the text itself. Each character is one of the first $c$ uppercase letters of the Latin alphabet.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2^{18}$ and the sum of $2^c$ over all test cases does not exceed $2^{18}$.</p>

## Output

<p>For each test case, output a single line consisting of a single integer&nbsp;！ the minimum number of cases in the language.</p>





```input1|2,3,6,7,10,11,14,15
7
5 5 1
ABCDE
3 1 2
AAA
3 2 2
AAB
10 2 2
ABABABABAB
4 4 4
DCBA
1 17 1
Q
9 3 2
ABCABCABC
```




```output1
5
1
2
1
1
1
2
```



## Note

<p>In the first test case, there must be five cases in the language (for each of the letters <span class="tex-font-style-tt">'A'</span>, <span class="tex-font-style-tt">'B'</span>, <span class="tex-font-style-tt">'C'</span>, <span class="tex-font-style-tt">'D'</span>, and <span class="tex-font-style-tt">'E'</span> there must be a case that has a corresponding ending).</p><p>In the fourth test case, one case with ending <span class="tex-font-style-tt">'B'</span> is sufficient. </p>
