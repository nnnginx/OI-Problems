## Description

<div><p>The Berland Kingdom is a set of <span class="tex-span"><i>n</i></span> cities connected with each other with <span class="tex-span"><i>n</i> - 1</span> railways. Each road connects exactly two different cities. The capital is located in city <span class="tex-span">1</span>. For each city there is a way to get from there to the capital by rail.</p><p>In the <span class="tex-span"><i>i</i></span>-th city there is a soldier division number <span class="tex-span"><i>i</i></span>, each division is characterized by a number of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. It represents the priority, the smaller the number, the higher the priority of this division. All values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>One day the Berland King Berl Great declared a general mobilization, and for that, each division should arrive in the capital. Every day from every city except the capital a train departs. So there are exactly <span class="tex-span"><i>n</i> - 1</span> departing trains each day. Each train moves toward the capital and finishes movement on the opposite endpoint of the railway on the next day. It has some finite capacity of <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span>, expressed in the maximum number of divisions, which this train can transport in one go. Each train moves in the direction of reducing the distance to the capital. So each train passes exactly one railway moving from a city to the neighboring (where it stops) toward the capital.</p><p>In the first place among the divisions that are in the city, division with the smallest number of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> get on the train, then with the next smallest and so on, until either the train is full or all the divisions are be loaded. So it is possible for a division to stay in a city for a several days.</p><p>The duration of train's progress from one city to another is always equal to <span class="tex-span">1</span> day. All divisions start moving at the same time and end up in the capital, from where they don't go anywhere else any more. Each division moves along a simple path from its city to the capital, regardless of how much time this journey will take.</p><p>Your goal is to find for each division, in how many days it will arrive to the capital of Berland. The countdown begins from day <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>). It is the number of cities in Berland. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the priority of the division, located in the city number <span class="tex-span"><i>i</i></span>. All numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are different (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Then <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of the railway roads. Each description consists of three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub>, <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>c</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> are number of cities connected by the <span class="tex-span"><i>j</i></span>-th rail, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> stands for the maximum capacity of a train riding on this road (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>u</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≠ <i>u</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>). </p></div><div class="output-specification"><p>Print sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of days it takes for the division of city <span class="tex-span"><i>i</i></span> to arrive to the capital. Separate numbers with spaces.</p></div>


## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>). It is the number of cities in Berland. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the priority of the division, located in the city number <span class="tex-span"><i>i</i></span>. All numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are different (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Then <span class="tex-span"><i>n</i> - 1</span> lines contain the descriptions of the railway roads. Each description consists of three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub>, <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>c</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> are number of cities connected by the <span class="tex-span"><i>j</i></span>-th rail, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> stands for the maximum capacity of a train riding on this road (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>u</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≠ <i>u</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>). </p>


## Output

<p>Print sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of days it takes for the division of city <span class="tex-span"><i>i</i></span> to arrive to the capital. Separate numbers with spaces.</p>


## Samples

```input1
4
40 10 30 20
1 2 1
2 3 1
4 2 1

```

```output1
0 1 3 2
```






```input2
5
5 4 3 2 1
1 2 1
2 3 1
2 4 1
4 5 1

```

```output2
0 1 4 2 3
```



