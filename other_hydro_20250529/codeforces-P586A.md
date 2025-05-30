## Description

<div><p>Alena has successfully passed the entrance exams to the university and is now looking forward to start studying.</p><p>One two-hour lesson at the Russian university is traditionally called a <span class="tex-font-style-it">pair</span>, it lasts for two academic hours (an academic hour is equal to 45 minutes).</p><p>The University works in such a way that every day it holds exactly <span class="tex-span"><i>n</i></span> lessons. Depending on the schedule of a particular group of students, on a given day, some pairs may actually contain classes, but some may be empty (such pairs are called breaks).</p><p>The official website of the university has already published the schedule for tomorrow for Alena's group. Thus, for each of the <span class="tex-span"><i>n</i></span> pairs she knows if there will be a class at that time or not.</p><p>Alena's House is far from the university, so if there are breaks, she doesn't always go home. Alena has time to go home only if the break consists of at least two free pairs in a row, otherwise she waits for the next pair at the university.</p><p>Of course, Alena does not want to be sleepy during pairs, so she will sleep as long as possible, and will only come to the first pair that is presented in her schedule. Similarly, if there are no more pairs, then Alena immediately goes home.</p><p>Alena appreciates the time spent at home, so she always goes home when it is possible, and returns to the university only at the beginning of the next pair. Help Alena determine for how many pairs she will stay at the university. Note that during some pairs Alena may be at the university waiting for the upcoming pair.</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of lessons at the university. </p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>, if Alena doesn't have the <span class="tex-span"><i>i</i></span>-th pairs, otherwise it is equal to <span class="tex-span">1</span>. Numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are separated by spaces.</p></div><div class="output-specification"><p>Print a single number — the number of pairs during which Alena stays at the university.</p></div>


## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of lessons at the university. </p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>). Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>, if Alena doesn't have the <span class="tex-span"><i>i</i></span>-th pairs, otherwise it is equal to <span class="tex-span">1</span>. Numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are separated by spaces.</p>


## Output

<p>Print a single number — the number of pairs during which Alena stays at the university.</p>


## Samples

```input1
5
0 1 0 1 1

```

```output1
4

```






```input2
7
1 0 1 0 0 1 0

```

```output2
4

```






```input3
1
0

```

```output3
0

```




## Note

<p>In the first sample Alena stays at the university from the second to the fifth pair, inclusive, during the third pair she will be it the university waiting for the next pair. </p><p>In the last sample Alena doesn't have a single pair, so she spends all the time at home.</p>

