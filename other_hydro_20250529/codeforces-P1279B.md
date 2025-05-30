## Description

<div><p>New Year is coming! Vasya has prepared a New Year's verse and wants to recite it in front of Santa Claus.</p><p>Vasya's verse contains $n$ parts. It takes $a_i$ seconds to recite the $i$-th part. Vasya can't change the order of parts in the verse: firstly he recites the part which takes $a_1$ seconds, secondly ！ the part which takes $a_2$ seconds, and so on. After reciting the verse, Vasya will get the number of presents equal to the number of parts he fully recited.</p><p>Vasya can skip at most one part of the verse while reciting it (if he skips more than one part, then Santa will definitely notice it).</p><p>Santa will listen to Vasya's verse for no more than $s$ seconds. For example, if $s = 10$, $a = [100, 9, 1, 1]$, and Vasya skips the first part of verse, then he gets two presents.</p><p>Note that it is possible to recite the whole verse (if there is enough time). </p><p>Determine which part Vasya needs to skip to obtain the maximum possible number of gifts. If Vasya shouldn't skip anything, print <span class="tex-font-style-tt">0</span>. If there are multiple answers, print any of them.</p><p>You have to process $t$ test cases.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) ！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $s$ ($1 \le n \le 10^5, 1 \le s \le 10^9$) ！ the number of parts in the verse and the maximum number of seconds Santa will listen to Vasya, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) ！ the time it takes to recite each part of the verse.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print one integer ！ the number of the part that Vasya needs to skip to obtain the maximum number of gifts. If Vasya shouldn't skip any parts, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) ！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $s$ ($1 \le n \le 10^5, 1 \le s \le 10^9$) ！ the number of parts in the verse and the maximum number of seconds Santa will listen to Vasya, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) ！ the time it takes to recite each part of the verse.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print one integer ！ the number of the part that Vasya needs to skip to obtain the maximum number of gifts. If Vasya shouldn't skip any parts, print <span class="tex-font-style-tt">0</span>.</p>

## Samples

```input1
3
7 11
2 9 1 3 18 1 4
4 35
11 9 10 7
1 8
5
```

```output1
2
1
0
```




## Note

<p>In the first test case if Vasya skips the second part then he gets three gifts.</p><p>In the second test case no matter what part of the verse Vasya skips.</p><p>In the third test case Vasya can recite the whole verse.</p>
