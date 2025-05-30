## Description

<div><p>When Petya has free from computer games time, he attends university classes. Every day the lessons on Petya’s faculty consist of two double classes. The floor where the lessons take place is a long corridor with <span class="tex-span"><i>M</i></span> classrooms numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>M</i></span>, situated along it.</p><p>All the students of Petya’s year are divided into <span class="tex-span"><i>N</i></span> groups. Petya has noticed recently that these groups’ timetable has the following peculiarity: the number of the classroom where the first lesson of a group takes place does not exceed the number of the classroom where the second lesson of this group takes place. </p><p>Once Petya decided to count the number of ways in which one can make a lesson timetable for all these groups. The timetable is a set of <span class="tex-span">2<i>N</i></span> numbers: for each group the number of the rooms where the first and the second lessons take place. Unfortunately, he quickly lost the track of his calculations and decided to count only the timetables that satisfy the following conditions:</p><p>1) On the first lesson in classroom <span class="tex-span"><i>i</i></span> exactly <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span> groups must be present.</p><p>2) In classroom <span class="tex-span"><i>i</i></span> no more than <span class="tex-span"><i>Y</i><sub class="lower-index"><i>i</i></sub></span> groups may be placed.</p><p>Help Petya count the number of timetables satisfying all those conditionsю As there can be a lot of such timetables, output modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>M</i> ≤ 100</span>) — the number of classrooms.</p><p>The second line contains <span class="tex-span"><i>M</i></span> space-separated integers — <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>X</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) the amount of groups present in classroom <span class="tex-span"><i>i</i></span> during the first lesson.</p><p>The third line contains <span class="tex-span"><i>M</i></span> space-separated integers — <span class="tex-span"><i>Y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>Y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) the maximal amount of groups that can be present in classroom <span class="tex-span"><i>i</i></span> at the same time.</p><p>It is guaranteed that all the <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub> ≤ <i>Y</i><sub class="lower-index"><i>i</i></sub></span>, and that the sum of all the <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span> is positive and does not exceed <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>In the single line output the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>


## Input

<p>The first line contains one integer <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>M</i> ≤ 100</span>) — the number of classrooms.</p><p>The second line contains <span class="tex-span"><i>M</i></span> space-separated integers — <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>X</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) the amount of groups present in classroom <span class="tex-span"><i>i</i></span> during the first lesson.</p><p>The third line contains <span class="tex-span"><i>M</i></span> space-separated integers — <span class="tex-span"><i>Y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>Y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) the maximal amount of groups that can be present in classroom <span class="tex-span"><i>i</i></span> at the same time.</p><p>It is guaranteed that all the <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub> ≤ <i>Y</i><sub class="lower-index"><i>i</i></sub></span>, and that the sum of all the <span class="tex-span"><i>X</i><sub class="lower-index"><i>i</i></sub></span> is positive and does not exceed <span class="tex-span">1000</span>.</p>


## Output

<p>In the single line output the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>


## Samples

```input1
3
1 1 1
1 2 3

```

```output1
36

```






```input2
3
1 1 1
1 1 1

```

```output2
6

```




## Note

<p>In the second sample test the first and the second lessons of each group must take place in the same classroom, that’s why the timetables will only be different in the rearrangement of the classrooms’ numbers for each group, e.g. <span class="tex-span">3! = 6</span>.</p>

