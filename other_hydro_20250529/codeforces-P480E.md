## Description

<div><p>Petya's been bored at work and he is killing the time by watching the parking lot at the office. The parking lot looks from above like an <span class="tex-span"><i>n</i> × <i>m</i></span> table (a cell of the table corresponds to a single parking spot). Some spots in the parking lot are taken, others are empty.</p><p>Petya watches cars riding into the parking lot one by one. After a car settles down at the parking spot, Petya amuzes himself by counting what maximum square of empty spots (i.e. a square subtable) can be seen on the parking lot if we look at it from above. Also, he takes notes of the square's size (side length) in his notebook. </p><p>You task is: given the state of the parking lot at the initial moment of time and the information about where the arriving cars park, restore what Petya wrote in his notebook. It is midday, so nobody leaves the lot.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> — the sizes of the parking lot and the number of arriving cars after Petya started his watch (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 2000</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters '<span class="tex-font-style-tt">X</span>' and '.', where '<span class="tex-font-style-tt">X</span>' means a taken spot and '.' means an empty spot. Each of the next <span class="tex-span"><i>k</i></span> lines contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> — the number of row and column of the spot the corresponding car takes (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>). It is guaranteed that this place was empty. You can assume that a car enters a parking lot only after the previous car successfully finds a spot.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> integers — the length of the side of the maximum square of empty spots after the corresponding car has entered the parking lot.</p></div>


## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> — the sizes of the parking lot and the number of arriving cars after Petya started his watch (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 2000</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters '<span class="tex-font-style-tt">X</span>' and '.', where '<span class="tex-font-style-tt">X</span>' means a taken spot and '.' means an empty spot. Each of the next <span class="tex-span"><i>k</i></span> lines contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> — the number of row and column of the spot the corresponding car takes (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>). It is guaranteed that this place was empty. You can assume that a car enters a parking lot only after the previous car successfully finds a spot.</p>


## Output

<p>Print <span class="tex-span"><i>k</i></span> integers — the length of the side of the maximum square of empty spots after the corresponding car has entered the parking lot.</p>


## Samples

```input1
7 8 4
........
X.....X.
........
........
.X......
........
........
1 5
6 4
3 5
4 6

```

```output1
5
4
4
3

```



