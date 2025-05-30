## Description

<div><p>Mad scientist Mike has applied for a job. His task is to manage a system of water pumping stations.</p><p>The system consists of <span class="tex-span"><i>n</i></span> pumping stations, which are numbered by integers from 1 to <span class="tex-span"><i>n</i></span>. Some pairs of stations are connected by bidirectional pipes through which water can flow in either direction (but only in one at a time). For each pipe you know its bandwidth — the maximum number of liters of water that can flow through it in one hour. Each pumping station can pump incoming water from some stations to other stations through the pipes, provided that in one hour the total influx of water to the station is equal to the total outflux of water from the station.</p><p>It is Mike's responsibility to pump water between stations. From station <span class="tex-span"><i>a</i></span> to station <span class="tex-span"><i>b</i></span> through the pipes (possibly through other stations) within one hour one can transmit a certain number of liters of water according to the rules described above. During this time, water from other stations can not flow into station <span class="tex-span"><i>a</i></span>, and can not flow out of the station <span class="tex-span"><i>b</i></span>. However, any amount of water can flow out of station <span class="tex-span"><i>a</i></span> or in station <span class="tex-span"><i>b</i></span>. If a total of <span class="tex-span"><i>x</i></span> litres of water flows out of the station <span class="tex-span"><i>a</i></span> in an hour, then Mike gets <span class="tex-span"><i>x</i></span> bollars more to his salary.</p><p>To get paid, Mike needs to work for <span class="tex-span"><i>n</i> - 1</span> days, according to the contract. On the first day he selects two stations <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, and within one hour he pumps a certain amount of water from <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>. Next, on the <span class="tex-span"><i>i</i></span>-th day Mike chooses a station <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> that has been never selected before, and pumps a certain amount of water out of the station <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to station <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> for one hour. The quantity of water he pumps on the <span class="tex-span"><i>i</i></span>-th day <span class="tex-font-style-bf">does not depend</span> on the amount of water pumped on the <span class="tex-span">(<i>i</i> - 1)</span>-th day.</p><p>Mike needs to earn as much bollars as he can for his projects. Help Mike find such a permutation of station numbers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>n</i></sub></span> so Mike will be able to earn the highest possible salary.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of stations and pipes in the system, accordingly. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the numbers of stations connected by the <span class="tex-span"><i>i</i></span>-th pipe and the pipe's bandwidth, accordingly. It is guaranteed that any two stations are connected by at most one pipe and that there is a pipe path between any two stations.</p></div><div class="output-specification"><p>On the first line print a single integer — the maximum salary Mike can earn.</p><p>On the second line print a space-separated permutation of <span class="tex-span"><i>n</i></span> numbers from 1 to <span class="tex-span"><i>n</i></span> — the numbers of stations in the sequence <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>n</i></sub></span>. If there are multiple answers, print any of them.</p></div>


## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of stations and pipes in the system, accordingly. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the numbers of stations connected by the <span class="tex-span"><i>i</i></span>-th pipe and the pipe's bandwidth, accordingly. It is guaranteed that any two stations are connected by at most one pipe and that there is a pipe path between any two stations.</p>


## Output

<p>On the first line print a single integer — the maximum salary Mike can earn.</p><p>On the second line print a space-separated permutation of <span class="tex-span"><i>n</i></span> numbers from 1 to <span class="tex-span"><i>n</i></span> — the numbers of stations in the sequence <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>n</i></sub></span>. If there are multiple answers, print any of them.</p>


## Samples

```input1
6 11
1 2 10
1 6 8
2 3 4
2 5 2
2 6 3
3 4 5
3 5 4
3 6 2
4 5 7
4 6 2
5 6 3

```

```output1
77
6 2 1 5 3 4 

```



