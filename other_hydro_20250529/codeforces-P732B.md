## Description

<div><p>Recently a dog was bought for Polycarp. The dog's name is Cormen. Now Polycarp has a lot of troubles. For example, Cormen likes going for a walk. </p><p>Empirically Polycarp learned that the dog needs at least <span class="tex-span"><i>k</i></span> walks for any two consecutive days in order to feel good. For example, if <span class="tex-span"><i>k</i> = 5</span> and yesterday Polycarp went for a walk with Cormen <span class="tex-span">2</span> times, today he has to go for a walk at least <span class="tex-span">3</span> times. </p><p>Polycarp analysed all his affairs over the next <span class="tex-span"><i>n</i></span> days and made a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of times Polycarp will walk with the dog on the <span class="tex-span"><i>i</i></span>-th day while doing all his affairs (for example, he has to go to a shop, throw out the trash, etc.).</p><p>Help Polycarp determine the minimum number of walks he needs to do additionaly in the next <span class="tex-span"><i>n</i></span> days so that Cormen will feel good during all the <span class="tex-span"><i>n</i></span> days. You can assume that on the day before the first day and on the day after the <span class="tex-span"><i>n</i></span>-th day Polycarp will go for a walk with Cormen exactly <span class="tex-span"><i>k</i></span> times. </p><p>Write a program that will find the minumum number of additional walks and the appropriate schedule&nbsp;— the sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means the total number of walks with the dog on the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 500</span>)&nbsp;— the number of days and the minimum number of walks with Cormen for any two consecutive days. </p><p>The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>)&nbsp;— the number of walks with Cormen on the <span class="tex-span"><i>i</i></span>-th day which Polycarp has already planned. </p></div><div class="output-specification"><p>In the first line print the smallest number of additional walks that Polycarp should do during the next <span class="tex-span"><i>n</i></span> days so that Cormen will feel good during all days. </p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the total number of walks on the <span class="tex-span"><i>i</i></span>-th day according to the found solutions (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i></span>). If there are multiple solutions, print any of them. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 500</span>)&nbsp;— the number of days and the minimum number of walks with Cormen for any two consecutive days. </p><p>The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>)&nbsp;— the number of walks with Cormen on the <span class="tex-span"><i>i</i></span>-th day which Polycarp has already planned. </p>

## Output

<p>In the first line print the smallest number of additional walks that Polycarp should do during the next <span class="tex-span"><i>n</i></span> days so that Cormen will feel good during all days. </p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the total number of walks on the <span class="tex-span"><i>i</i></span>-th day according to the found solutions (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i></span>). If there are multiple solutions, print any of them. </p>

## Samples

```input1
3 5
2 0 1

```

```output1
4
2 3 2

```






```input2
3 1
0 0 0

```

```output2
1
0 1 0

```






```input3
4 6
2 4 3 5

```

```output3
0
2 4 3 5

```



