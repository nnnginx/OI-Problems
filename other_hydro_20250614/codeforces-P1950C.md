## Description

<div><p>Given the time in 24-hour format, output the equivalent time in 12-hour format. </p><ul> <li> <a href="https://en.wikipedia.org/wiki/24-hour_clock#Description">24-hour format</a> divides the day into 24 hours from $00$ to $23$, each of which has 60 minutes from $00$ to $59$. </li><li> <a href="https://en.wikipedia.org/wiki/12-hour_clock#Description">12-hour format</a> divides the day into two halves: the first half is $\mathrm{AM}$, and the second half is $\mathrm{PM}$. In each half, the hours are numbered in the order $12, 01, 02, 03, \dots, 11$. Each hour has 60 minutes numbered from $00$ to $59$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1440$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains a string $s$ of length $5$ with format <span class="tex-font-style-tt">hh:mm</span> representing a valid time in the 24-hour format. <span class="tex-font-style-tt">hh</span> represents the hour from $00$ to $23$, and <span class="tex-font-style-tt">mm</span> represents the minute from $00$ to $59$.</p><p>The input will always be a valid time in 24-hour format.</p></div><div class="output-specification"><p>For each test case, output two strings separated by a space ("<span class="tex-font-style-tt">hh:mm AM</span>" or "<span class="tex-font-style-tt">hh:mm PM</span>"), which are the 12-hour equivalent to the time provided in the test case (without quotes).</p><p>You should output the time exactly as indicated; in particular, you should not remove leading zeroes.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1440$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains a string $s$ of length $5$ with format <span class="tex-font-style-tt">hh:mm</span> representing a valid time in the 24-hour format. <span class="tex-font-style-tt">hh</span> represents the hour from $00$ to $23$, and <span class="tex-font-style-tt">mm</span> represents the minute from $00$ to $59$.</p><p>The input will always be a valid time in 24-hour format.</p>

## Output

<p>For each test case, output two strings separated by a space ("<span class="tex-font-style-tt">hh:mm AM</span>" or "<span class="tex-font-style-tt">hh:mm PM</span>"), which are the 12-hour equivalent to the time provided in the test case (without quotes).</p><p>You should output the time exactly as indicated; in particular, you should not remove leading zeroes.</p>





```input1|2,4,6,8,10,12
11
09:41
18:06
12:14
00:59
00:00
14:34
01:01
19:07
11:59
12:00
21:37
```




```output1
09:41 AM
06:06 PM
12:14 PM
12:59 AM
12:00 AM
02:34 PM
01:01 AM
07:07 PM
11:59 AM
12:00 PM
09:37 PM
```


