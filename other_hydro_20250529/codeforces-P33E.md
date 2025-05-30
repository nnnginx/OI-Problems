## Description

<div><p>It's unbelievable, but an exam period has started at the OhWord University. It's even more unbelievable, that Valera got all the tests before the exam period for excellent work during the term. As now he's free, he wants to earn money by solving problems for his groupmates. He's made a <span class="tex-span"><i>list</i></span> of subjects that he can help with. Having spoken with <span class="tex-span"><i>n</i></span> of his groupmates, Valera found out the following information about them: what subject each of them passes, time of the exam and sum of money that each person is ready to pay for Valera's help.</p><p>Having this data, Valera's decided to draw up a timetable, according to which he will solve problems for his groupmates. For sure, Valera can't solve problems round the clock, that's why he's found for himself an optimum order of day and plans to stick to it during the whole exam period. Valera assigned time segments for sleep, breakfast, lunch and dinner. The rest of the time he can work.</p><p>Obviously, Valera can help a student with some subject, only if this subject is on the <span class="tex-span"><i>list</i></span>. It happened, that all the students, to whom Valera spoke, have different, but one-type problems, that's why Valera can solve any problem of subject <span class="tex-span"><i>list</i><sub class="lower-index"><i>i</i></sub></span> in <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes.</p><p>Moreover, if Valera starts working at some problem, he can break off only for sleep or meals, but he can't start a new problem, not having finished the current one. Having solved the problem, Valera can send it instantly to the corresponding student via the Internet.</p><p>If this student's exam hasn't started yet, he can make a crib, use it to pass the exam successfully, and pay Valera the promised sum. Since Valera has little time, he asks you to write a program that finds the order of solving problems, which can bring Valera maximum profit.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>m</i>, <i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 30</span>) — amount of subjects on the <span class="tex-span"><i>list</i></span>, amount of Valera's potential employers and the duration of the exam period in days.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the names of subjects <span class="tex-span"><i>list</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>list</i><sub class="lower-index"><i>i</i></sub></span> is a non-empty string of at most 32 characters, consisting of lower case Latin letters). It's guaranteed that no two subjects are the same.</p><p>The <span class="tex-span">(<i>m</i> + 2)</span>-th line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — time in minutes that Valera spends to solve problems of the <span class="tex-span"><i>i</i></span>-th subject. Then follow four lines, containing time segments for sleep, breakfast, lunch and dinner correspondingly.</p><p>Each line is in format <span class="tex-font-style-tt">H1:M1-H2:M2</span>, where <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">H1</span>, <span class="tex-font-style-tt">H2</span> <span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">M1</span>, <span class="tex-font-style-tt">M2</span> <span class="tex-span"> ≤ 59</span>. Time <span class="tex-font-style-tt">H1:M1</span> stands for the first minute of some Valera's action, and time <span class="tex-font-style-tt">H2:M2</span> stands for the last minute of this action. No two time segments cross. It's guaranteed that Valera goes to bed before midnight, gets up earlier than he has breakfast, finishes his breakfast before lunch, finishes his lunch before dinner, and finishes his dinner before midnight. All these actions last less than a day, but not less than one minute. Time of the beginning and time of the ending of each action are within one and the same day. But it's possible that Valera has no time for solving problems.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing the description of students. For each student the following is known: his exam subject <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a non-empty string of at most 32 characters, consisting of lower case Latin letters), index of the exam day <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>), the exam time <span class="tex-span"><i>time</i><sub class="lower-index"><i>i</i></sub></span>, and sum of money <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — integer) that he's ready to pay for Valera's help. Exam time <span class="tex-span"><i>time</i><sub class="lower-index"><i>i</i></sub></span> is in the format <span class="tex-font-style-tt">HH:MM</span>, where <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">HH</span> <span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">MM</span> <span class="tex-span"> ≤ 59</span>. Valera will get money, if he finishes to solve the problem strictly before the corresponding student's exam begins.</p></div><div class="output-specification"><p>In the first line output the maximum profit that Valera can get. The second line should contain number <span class="tex-span"><i>p</i></span> — amount of problems that Valera is to solve. In the following <span class="tex-span"><i>p</i></span> lines output the order of solving problems in chronological order in the following format: index of a student, to whom Valera is to help; index of the time, when Valera should start the problem; time, when Valera should start the problem (the first minute of his work); index of the day, when Valera should finish the problem; time, when Valera should finish the problem (the last minute of his work). To understand the output format better, study the sample tests.</p></div>


## Input

<p>The first line contains integers <span class="tex-span"><i>m</i>, <i>n</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 30</span>) — amount of subjects on the <span class="tex-span"><i>list</i></span>, amount of Valera's potential employers and the duration of the exam period in days.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the names of subjects <span class="tex-span"><i>list</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>list</i><sub class="lower-index"><i>i</i></sub></span> is a non-empty string of at most 32 characters, consisting of lower case Latin letters). It's guaranteed that no two subjects are the same.</p><p>The <span class="tex-span">(<i>m</i> + 2)</span>-th line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — time in minutes that Valera spends to solve problems of the <span class="tex-span"><i>i</i></span>-th subject. Then follow four lines, containing time segments for sleep, breakfast, lunch and dinner correspondingly.</p><p>Each line is in format <span class="tex-font-style-tt">H1:M1-H2:M2</span>, where <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">H1</span>, <span class="tex-font-style-tt">H2</span> <span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">M1</span>, <span class="tex-font-style-tt">M2</span> <span class="tex-span"> ≤ 59</span>. Time <span class="tex-font-style-tt">H1:M1</span> stands for the first minute of some Valera's action, and time <span class="tex-font-style-tt">H2:M2</span> stands for the last minute of this action. No two time segments cross. It's guaranteed that Valera goes to bed before midnight, gets up earlier than he has breakfast, finishes his breakfast before lunch, finishes his lunch before dinner, and finishes his dinner before midnight. All these actions last less than a day, but not less than one minute. Time of the beginning and time of the ending of each action are within one and the same day. But it's possible that Valera has no time for solving problems.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing the description of students. For each student the following is known: his exam subject <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a non-empty string of at most 32 characters, consisting of lower case Latin letters), index of the exam day <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>), the exam time <span class="tex-span"><i>time</i><sub class="lower-index"><i>i</i></sub></span>, and sum of money <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — integer) that he's ready to pay for Valera's help. Exam time <span class="tex-span"><i>time</i><sub class="lower-index"><i>i</i></sub></span> is in the format <span class="tex-font-style-tt">HH:MM</span>, where <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">HH</span> <span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">MM</span> <span class="tex-span"> ≤ 59</span>. Valera will get money, if he finishes to solve the problem strictly before the corresponding student's exam begins.</p>


## Output

<p>In the first line output the maximum profit that Valera can get. The second line should contain number <span class="tex-span"><i>p</i></span> — amount of problems that Valera is to solve. In the following <span class="tex-span"><i>p</i></span> lines output the order of solving problems in chronological order in the following format: index of a student, to whom Valera is to help; index of the time, when Valera should start the problem; time, when Valera should start the problem (the first minute of his work); index of the day, when Valera should finish the problem; time, when Valera should finish the problem (the last minute of his work). To understand the output format better, study the sample tests.</p>


## Samples

```input1
3 3 4
calculus
algebra
history
58 23 15
00:00-08:15
08:20-08:35
09:30-10:25
19:00-19:45
calculus 1 09:36 100
english 4 21:15 5000
history 1 19:50 50

```

```output1
150
2
1 1 08:16 1 09:29
3 1 10:26 1 10:40

```






```input2
2 2 1
matan
codeforces
1 2
00:00-08:00
09:00-09:00
12:00-12:00
18:00-18:00
codeforces 1 08:04 2
matan 1 08:02 1

```

```output2
3
2
2 1 08:01 1 08:01
1 1 08:02 1 08:03

```






```input3
2 2 1
matan
codeforces
2 2
00:00-08:00
09:00-09:00
12:00-12:00
18:00-18:00
codeforces 1 08:04 2
matan 1 08:03 1

```

```output3
2
1
1 1 08:01 1 08:02

```



