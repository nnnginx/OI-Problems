## Description

<div><p>Athenaeus has just finished creating his latest musical composition and will present it tomorrow to the people of Athens. Unfortunately, the melody is rather dull and highly likely won't be met with a warm reception. </p><p>His song consists of $n$ notes, which we will treat as <span class="tex-font-style-bf">positive integers</span>. The <span class="tex-font-style-bf">diversity</span> of a song is the number of <span class="tex-font-style-bf">different</span> notes it contains. As a patron of music, Euterpe watches over composers and guides them throughout the process of creating new melodies. She decided to help Athenaeus by changing his song to make it more diverse.</p><p>Being a minor goddess, she cannot arbitrarily change the song. Instead, for each of the $n$ notes in the song, she can either leave it as it is or <span class="tex-font-style-bf">increase</span> it by $1$.</p><p>Given the song as a sequence of integers describing the notes, find out the maximal, achievable diversity.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;�� the number of test cases. Then $t$ test cases follow, each one is described in two lines.</p><p>In the first line of each test case there is a single integer $n$ ($1 \leq n \leq 10^5$) denoting the length of the song. The next line contains a sequence of $n$ integers $x_1, x_2, \ldots, x_n$ $(1 \leq x_1 \leq x_2 \leq \ldots \leq x_n \leq 2 \cdot n)$, describing the song.</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, you should output a single line containing precisely one integer, the maximal diversity of the song, i.e. the maximal possible number of different elements in the final sequence.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;�� the number of test cases. Then $t$ test cases follow, each one is described in two lines.</p><p>In the first line of each test case there is a single integer $n$ ($1 \leq n \leq 10^5$) denoting the length of the song. The next line contains a sequence of $n$ integers $x_1, x_2, \ldots, x_n$ $(1 \leq x_1 \leq x_2 \leq \ldots \leq x_n \leq 2 \cdot n)$, describing the song.</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, you should output a single line containing precisely one integer, the maximal diversity of the song, i.e. the maximal possible number of different elements in the final sequence.</p>

## Samples

```input1
5
6
1 2 2 2 5 6
2
4 4
6
1 1 3 4 4 5
1
1
6
1 1 1 2 2 2
```

```output1
5
2
6
1
3
```




## Note

<p>In the first test case, Euterpe can increase the second, fifth and sixth element to obtain the sequence $1, \underline{3}, 2, 2, \underline{6}, \underline{7}$, which has $5$ different elements (increased elements are underlined).</p><p>In the second test case, Euterpe can increase the first element to obtain the sequence $\underline{5}, 4$, which has $2$ different elements.</p><p>In the third test case, Euterpe can increase the second, fifth and sixth element to obtain the sequence $1, \underline{2}, 3, 4, \underline{5}, \underline{6}$, which has $6$ different elements.</p>
