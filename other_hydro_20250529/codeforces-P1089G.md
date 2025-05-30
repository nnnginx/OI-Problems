## Description

<div><p>Berland State University invites people from all over the world as guest students. You can come to the capital of Berland and study with the best teachers in the country.</p><p>Berland State University works every day of the week, but classes for guest students are held on the following schedule. You know the sequence of seven integers $a_1, a_2, \dots, a_7$ ($a_i = 0$ or $a_i = 1$):</p><ul> <li> $a_1=1$ if and only if there are classes for guest students on Sundays; </li><li> $a_2=1$ if and only if there are classes for guest students on Mondays; </li><li> ...  </li><li> $a_7=1$ if and only if there are classes for guest students on Saturdays. </li></ul><p>The classes for guest students are held in at least one day of a week.</p><p>You want to visit the capital of Berland and spend the minimum number of days in it to study $k$ days as a guest student in Berland State University. Write a program to find the length of the shortest continuous period of days to stay in the capital to study exactly $k$ days as a guest student.</p></div><div class="input-specification"><p>The first line of the input contains integer $t$ ($1 \le t \le 10\,000$) ！ the number of test cases to process. For each test case independently solve the problem and print the answer. </p><p>Each test case consists of two lines. The first of them contains integer $k$ ($1 \le k \le 10^8$) ！ the required number of days to study as a guest student. The second line contains exactly seven integers $a_1, a_2, \dots, a_7$ ($a_i = 0$ or $a_i = 1$) where $a_i=1$ if and only if classes for guest students are held on the $i$-th day of a week.</p></div><div class="output-specification"><p>Print $t$ lines, the $i$-th line should contain the answer for the $i$-th test case ！ the length of the shortest continuous period of days you need to stay to study exactly $k$ days as a guest student.</p></div>

## Input

<p>The first line of the input contains integer $t$ ($1 \le t \le 10\,000$) ！ the number of test cases to process. For each test case independently solve the problem and print the answer. </p><p>Each test case consists of two lines. The first of them contains integer $k$ ($1 \le k \le 10^8$) ！ the required number of days to study as a guest student. The second line contains exactly seven integers $a_1, a_2, \dots, a_7$ ($a_i = 0$ or $a_i = 1$) where $a_i=1$ if and only if classes for guest students are held on the $i$-th day of a week.</p>

## Output

<p>Print $t$ lines, the $i$-th line should contain the answer for the $i$-th test case ！ the length of the shortest continuous period of days you need to stay to study exactly $k$ days as a guest student.</p>

## Samples

```input1
3
2
0 1 0 0 0 0 0
100000000
1 0 0 0 1 0 1
1
1 0 0 0 0 0 0
```

```output1
8
233333332
1
```




## Note

<p>In the first test case you must arrive to the capital of Berland on Monday, have classes on this day, spend a week until next Monday and have classes on the next Monday. In total you need to spend $8$ days in the capital of Berland.</p>
