<p>The <em>Warring States Period</em> (473-22l BC) refers to the centuries of turmoil following the Spring and
Autumn Period. China was divided into many little kingdoms that were constantly fighting with each
other. Unlike in previous ages, when chivalry played an important role in battles and the states fought
mostly for balance of power or to resolve disputes, in this period the aim of battle was to conquer and
completely annihilate the other states. Eventually seven states, known as the ``Seven Great Powers'' rose
to prominence: Qi, Chu, Yan, Han, Zhao, Wei, and Qin. After numerous alliances and counter-alliances,
Qin defeated all the other states one by one, putting an end to the Warring States Period.</p>
<p>You are given a map that shows the position of the capital for each state, and the borders between the
states as a series of line segments. Your job is to determine which states were fighting with each other.
This is pretty easy to determine - if two states had a common border, then they were fighting.</p>
<h3>Input</h3>
<p>The input contains several blocks of test cases. Each case begins with a line containing two integers:
the number 1&lt;= <i>n</i> &lt;=600 of states, and the number 1&lt;= <i>m</i> &lt;= 4000 of border segments. The next <i>n</i> lines describe the coordinates of capitals, there are two integers in each line. The next <i>m</i> lines after that
describe the <i>m</i> border segments. Each line contains four integers <i>x</i><sub><i>1</i></sub>, <i>y</i><sub><i>1</i></sub>,
<i>x</i><sub><i>2</i></sub> and <i>y</i><sub><i>2</i></sub> meaning that there is a border segment from (<i>x</i><sub><i>1</i></sub>, <i>y</i><sub><i>1</i></sub>) to (<i>x</i><sub><i>2</i></sub>, <i>y</i><sub><i>2</i></sub>).(It is not given in the input what the two states on the two sides of the border are, but it can be deduced from the way the borders go.)

</p><p>Each state is enclosed by a continuous borderline. The states are surrounded by an infinite wasteland,
thus a border segment either separates two states, or a state from the wasteland. It is not possible that
the same state is on both sides of a border segment, or the wasteland is on both sides of a border segment.
There is exactly one capital in each state, and there is no capital in the wasteland. The border segments
do not cross each other, they can meet only at the end points.</p>

<p>The input is terminated by a block with <i>n</i> = <i>m</i> = 0.</p>

<h3>Output</h3>

<p>For each test case, you have to output <i>n</i> lines that describe the enemies of the <i>n</i> states (recall that if two
states share a border, then they are enemies). Each line begins with an integer, the number <i>x</i> of enemies
the given state has. This number is followed by  <i>x</i> numbers identifying the enemies of the state. These
numbers are between 1 and <i>n</i> and number 1 refers to the first capital appearing in the input, number <i>n</i> refers to the last.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4 12
3 2
11 8
12 17
1 19
0 0 10 0
10 0 20 0
20 0 20 10
20 10 20 20
20 20 10 20
10 20 0 20
0 20 0 10
0 10 0 0
10 0 10 10
0 10 10 10
20 10 10 10
10 20 10 10
4 16
170 13
24 88
152 49
110 130
60 60 140 60
140 60 140 140
140 140 60 140
60 140 60 60
0 0 200 0
200 0 200 200
200 200 0 200
0 200 0 0
40 40 160 40
160 40 160 160
160 160 40 160
40 160 40 40
20 20 180 20
180 20 180 180
180 180 20 180
20 180 20 20
0 0

<b>Output:</b>
2 2 4
2 1 3
2 2 4
2 1 3
1 2
2 1 3
2 2 4
1 3
</pre>