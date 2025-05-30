## Description

<div><p>PMP is getting a warrior. He is practicing a lot, but the results are not acceptable yet. This time instead of programming contests, he decided to compete in a car racing to increase the spirit of victory. He decides to choose a competition that also exhibits algorithmic features.</p><p>AlgoRace is a special league of car racing where different teams compete in a country of <span class="tex-span"><i>n</i></span> cities. Cities are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Every two distinct cities in the country are connected with one bidirectional road. Each competing team should introduce one driver and a set of cars.</p><p>The competition is held in <span class="tex-span"><i>r</i></span> rounds. In <span class="tex-span"><i>i</i></span>-th round, drivers will start at city <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and finish at city <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Drivers are allowed to change their cars at most <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> times. Changing cars can take place in any city in no time. One car can be used multiple times in one round, but total number of changes should not exceed <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. Drivers can freely choose their path to destination.</p><p>PMP has prepared <span class="tex-span"><i>m</i></span> type of purpose-built cars. Beside for PMP’s driving skills, depending on properties of the car and the road, a car traverses each road in each direction in different times. </p><p>PMP Warriors wants to devise best strategies of choosing car and roads in each round to maximize the chance of winning the cup. For each round they want to find the minimum time required to finish it.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>r</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 60, 1 ≤ <i>m</i> ≤ 60, 1 ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities, the number of different types of cars and the number of rounds in the competition, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> sets of <span class="tex-span"><i>n</i> × <i>n</i></span> matrices of integers between <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span> (inclusive) will follow — describing the time one car requires to traverse different roads. The <span class="tex-span"><i>k</i></span>-th integer in <span class="tex-span"><i>j</i></span>-th line of the <span class="tex-span"><i>i</i></span>-th set is the time that <span class="tex-span"><i>i</i></span>-th car requires to traverse the road from <span class="tex-span"><i>j</i></span>-th city to <span class="tex-span"><i>k</i></span>-th city. These matrices are not necessarily symmetric, but their diagonal is always zero.</p><p>Next <span class="tex-span"><i>r</i></span> lines contain description of the rounds. The <span class="tex-span"><i>i</i></span>-th of these lines contains space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub>, 0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the number of starting city, finishing city and the number of possible car changes in <span class="tex-span"><i>i</i></span>-th round, correspondingly.</p></div><div class="output-specification"><p>For each round you should print the minimum required time to complete the round in a single line.</p></div>


## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>r</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 60, 1 ≤ <i>m</i> ≤ 60, 1 ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities, the number of different types of cars and the number of rounds in the competition, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> sets of <span class="tex-span"><i>n</i> × <i>n</i></span> matrices of integers between <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span> (inclusive) will follow — describing the time one car requires to traverse different roads. The <span class="tex-span"><i>k</i></span>-th integer in <span class="tex-span"><i>j</i></span>-th line of the <span class="tex-span"><i>i</i></span>-th set is the time that <span class="tex-span"><i>i</i></span>-th car requires to traverse the road from <span class="tex-span"><i>j</i></span>-th city to <span class="tex-span"><i>k</i></span>-th city. These matrices are not necessarily symmetric, but their diagonal is always zero.</p><p>Next <span class="tex-span"><i>r</i></span> lines contain description of the rounds. The <span class="tex-span"><i>i</i></span>-th of these lines contains space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub>, 0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the number of starting city, finishing city and the number of possible car changes in <span class="tex-span"><i>i</i></span>-th round, correspondingly.</p>


## Output

<p>For each round you should print the minimum required time to complete the round in a single line.</p>


## Samples

```input1
4 2 3
0 1 5 6
2 0 3 6
1 3 0 1
6 6 7 0
0 3 5 6
2 0 1 6
1 3 0 2
6 6 7 0
1 4 2
1 4 1
1 4 3

```

```output1
3
4
3

```






```input2
4 2 3
0 7 3 3
8 0 10 5
1 1 0 4
8 9 2 0
0 3 3 9
7 0 4 9
3 8 0 4
4 8 9 0
2 3 3
2 1 3
1 2 2

```

```output2
4
5
3

```




## Note

<p>In the first sample, in all rounds PMP goes from city #1 to city #2, then city #3 and finally city #4. But the sequences of types of the cars he uses are (1, 2, 1) in the first round and (1, 2, 2) in the second round. In the third round, although he can change his car three times, he uses the same strategy as the first round which only needs two car changes.</p>

