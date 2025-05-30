## Description

<div><p>In 2013, the writers of Berland State University should prepare problems for <span class="tex-span"><i>n</i></span> Olympiads. We will assume that the Olympiads are numbered with consecutive integers from 1 to <span class="tex-span"><i>n</i></span>. For each Olympiad we know how many members of the jury must be involved in its preparation, as well as the time required to prepare the problems for her. Namely, the Olympiad number <span class="tex-span"><i>i</i></span> should be prepared by <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> people for <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> days, the preparation for the Olympiad should be a continuous period of time and end exactly one day before the Olympiad. On the day of the Olympiad the juries who have prepared it, already do not work on it.</p><p>For example, if the Olympiad is held on December 9th and the preparation takes 7 people and 6 days, all seven members of the jury will work on the problems of the Olympiad from December, 3rd to December, 8th (the jury members won't be working on the problems of this Olympiad on December 9th, that is, some of them can start preparing problems for some other Olympiad). And if the Olympiad is held on November 3rd and requires 5 days of training, the members of the jury will work from October 29th to November 2nd.</p><p>In order not to overload the jury the following rule was introduced: one member of the jury can not work on the same day on the tasks for different Olympiads. Write a program that determines what the minimum number of people must be part of the jury so that all Olympiads could be prepared in time.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of Olympiads in 2013 (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the month and day of the Olympiad (given without leading zeroes), the needed number of the jury members and the time needed to prepare the <span class="tex-span"><i>i</i></span>-th Olympiad (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 12</span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed the number of days in month <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>. The Olympiads are given in the arbitrary order. Several Olympiads can take place in one day.</p><p>Use the modern (Gregorian) calendar in the solution. Note that all dates are given in the year 2013. This is not a leap year, so February has 28 days. <span class="tex-font-style-bf">Please note, the preparation of some Olympiad can start in 2012 year.</span></p></div><div class="output-specification"><p>Print a single number — the minimum jury size.</p></div>


## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of Olympiads in 2013 (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the month and day of the Olympiad (given without leading zeroes), the needed number of the jury members and the time needed to prepare the <span class="tex-span"><i>i</i></span>-th Olympiad (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 12</span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed the number of days in month <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>. The Olympiads are given in the arbitrary order. Several Olympiads can take place in one day.</p><p>Use the modern (Gregorian) calendar in the solution. Note that all dates are given in the year 2013. This is not a leap year, so February has 28 days. <span class="tex-font-style-bf">Please note, the preparation of some Olympiad can start in 2012 year.</span></p>


## Output

<p>Print a single number — the minimum jury size.</p>


## Samples

```input1
2
5 23 1 2
3 13 2 3

```

```output1
2

```






```input2
3
12 9 2 1
12 8 1 3
12 8 2 2

```

```output2
3

```






```input3
1
1 10 1 13

```

```output3
1

```



