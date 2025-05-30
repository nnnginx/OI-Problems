## Description

<div><p>In the last war of PMP, he defeated all his opponents and advanced to the final round. But after the end of semi-final round evil attacked him from behind and killed him! God bless him. </p><p>Before his death, PMP signed a contract with the bus rapid transit (BRT) that improves public transportations by optimizing time of travel estimation. You should help PMP finish his last contract.</p><p>Each BRT line is straight line that passes <span class="tex-span"><i>n</i></span> intersecting on its ways. At each intersection there is traffic light that periodically cycles between green and red. It starts illuminating green at time zero. During the green phase which lasts for <span class="tex-span"><i>g</i></span> seconds, traffic is allowed to proceed. After the green phase the light changes to red and remains in this color for <span class="tex-span"><i>r</i></span> seconds. During the red phase traffic is prohibited from proceeding. If a vehicle reaches the intersection exactly at a time when the light changes to red, it should stop, but the vehicle is clear to proceed if the light has just changed to green.</p><center> <img class="tex-graphics" src="./25964/file/LlrBAl6D.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>All traffic lights have the same timing and are synchronized. In other words the period of red (and green) phase is the same for all of traffic lights and they all start illuminating green at time zero.</p><p>The BRT Company has calculated the time that a bus requires to pass each road segment. A road segment is the distance between two consecutive traffic lights or between a traffic light and source (or destination) station. More precisely BRT specialists provide <span class="tex-span"><i>n</i> + 1</span> positive integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, the time in seconds that a bus needs to traverse <span class="tex-span"><i>i</i></span>-th road segment in the path from source to destination. The <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> value denotes the time that a bus needs to pass the distance between source and the first intersection. The <span class="tex-span"><i>l</i><sub class="lower-index"><i>n</i> + 1</sub></span> value denotes the time between the last intersection and destination.</p><p>In one day <span class="tex-span"><i>q</i></span> buses leave the source station. The <span class="tex-span"><i>i</i></span>-th bus starts from source at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (in seconds). Decision makers of BRT Company want to know what time a bus gets to destination?</p><p>The bus is considered as point. A bus will always move if it can. The buses do not interfere with each other. </p></div><div class="input-specification"><p>The first line of input contains three space-separated positive integers <span class="tex-span"><i>n</i>, <i>g</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>g</i> + <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of intersections, duration of green phase and duration of red phase. Next line contains <span class="tex-span"><i>n</i> + 1</span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the time to pass the <span class="tex-span"><i>i</i></span>-th road segment in the path from source to destination. </p><p>Next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of buses in a day. The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>q</i></span> lines contains a single integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the time when <span class="tex-span"><i>i</i></span>-th bus leaves the source station.</p></div><div class="output-specification"><p>In the <span class="tex-span"><i>i</i></span>-th line of output you should print a single integer — the time that <span class="tex-span"><i>i</i></span>-th bus gets to destination.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>


## Input

<p>The first line of input contains three space-separated positive integers <span class="tex-span"><i>n</i>, <i>g</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>g</i> + <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of intersections, duration of green phase and duration of red phase. Next line contains <span class="tex-span"><i>n</i> + 1</span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the time to pass the <span class="tex-span"><i>i</i></span>-th road segment in the path from source to destination. </p><p>Next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of buses in a day. The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>q</i></span> lines contains a single integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the time when <span class="tex-span"><i>i</i></span>-th bus leaves the source station.</p>


## Output

<p>In the <span class="tex-span"><i>i</i></span>-th line of output you should print a single integer — the time that <span class="tex-span"><i>i</i></span>-th bus gets to destination.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>


## Samples

```input1
1 3 2
5 2
5
1
2
3
4
5

```

```output1
8
9
12
12
12

```






```input2
5 3 7
10 1 1 8 900000005 1000000000
3
1
10
1000000000

```

```output2
1900000040
1900000040
2900000030

```




## Note

<p>In the first sample, buses #1, #2 and #5 will reach the destination without waiting behind the red light. But buses #3 and #4 should wait.</p><p>In the second sample, first bus should wait at third, fourth and fifth intersections. Second and third buses should wait only at the fifth intersection.</p>

