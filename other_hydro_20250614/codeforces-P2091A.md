## Description

<div><p>The final of the first Olympiad by IT Campus "NEIMARK" is scheduled for March 1, 2025. A nameless intern was tasked with forming the date of the Olympiad using digits&nbsp;！ 01.03.2025.</p><p>To accomplish this, the intern took a large bag of digits and began drawing them one by one. In total, he drew $n$ digits&nbsp;！ the digit $a_i$ was drawn in the $i$-th turn.</p><p>You suspect that the intern did extra work. Determine at which step the intern could have first assembled the digits to form the date of the Olympiad (the separating dots can be ignored), or report that it is impossible to form this date from the drawn digits. Note that leading zeros <span class="tex-font-style-bf">must be displayed</span>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 20$).</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 9$)&nbsp;！ the numbers that the intern pulled out in chronological order.</p></div><div class="output-specification"><p>For each test case, output the minimum number of digits that the intern could pull out. If all the digits cannot be used to make a date, output the number $0$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 20$).</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 9$)&nbsp;！ the numbers that the intern pulled out in chronological order.</p>

## Output

<p>For each test case, output the minimum number of digits that the intern could pull out. If all the digits cannot be used to make a date, output the number $0$.</p>





```input1|2,3,6,7
4
10
2 0 1 2 3 2 5 0 0 1
8
2 0 1 2 3 2 5 0
8
2 0 1 0 3 2 5 0
16
2 3 1 2 3 0 1 9 2 1 0 3 5 4 0 3
```




```output1
9
0
8
15
```


