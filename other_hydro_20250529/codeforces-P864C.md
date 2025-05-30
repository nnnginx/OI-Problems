## Description

<div><p>A bus moves along the coordinate line <span class="tex-span"><i>Ox</i></span> from the point <span class="tex-span"><i>x</i> = 0</span> to the point <span class="tex-span"><i>x</i> = <i>a</i></span>. After starting from the point <span class="tex-span"><i>x</i> = 0</span>, it reaches the point <span class="tex-span"><i>x</i> = <i>a</i></span>, immediately turns back and then moves to the point <span class="tex-span"><i>x</i> = 0</span>. After returning to the point <span class="tex-span"><i>x</i> = 0</span> it immediately goes back to the point <span class="tex-span"><i>x</i> = <i>a</i></span> and so on. Thus, the bus moves from <span class="tex-span"><i>x</i> = 0</span> to <span class="tex-span"><i>x</i> = <i>a</i></span> and back. Moving from the point <span class="tex-span"><i>x</i> = 0</span> to <span class="tex-span"><i>x</i> = <i>a</i></span> or from the point <span class="tex-span"><i>x</i> = <i>a</i></span> to <span class="tex-span"><i>x</i> = 0</span> is called a <span class="tex-font-style-it">bus journey</span>. In total, the bus must make <span class="tex-span"><i>k</i></span> journeys.</p><p>The petrol tank of the bus can hold <span class="tex-span"><i>b</i></span> liters of gasoline. To pass a single unit of distance the bus needs to spend exactly one liter of gasoline. The bus starts its first journey with a full petrol tank.</p><p>There is a gas station in point <span class="tex-span"><i>x</i> = <i>f</i></span>. This point is between points <span class="tex-span"><i>x</i> = 0</span> and <span class="tex-span"><i>x</i> = <i>a</i></span>. There are no other gas stations on the bus route. While passing by a gas station in either direction the bus can stop and completely refuel its tank. Thus, after stopping to refuel the tank will contain <span class="tex-span"><i>b</i></span> liters of gasoline.</p><p>What is the minimum number of times the bus needs to refuel at the point <span class="tex-span"><i>x</i> = <i>f</i></span> to make <span class="tex-span"><i>k</i></span> journeys? The first journey starts in the point <span class="tex-span"><i>x</i> = 0</span>.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 &lt; <i>f</i> &lt; <i>a</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>) — the endpoint of the first bus journey, the capacity of the fuel tank of the bus, the point where the gas station is located, and the required number of journeys.</p></div><div class="output-specification"><p>Print the minimum number of times the bus needs to refuel to make <span class="tex-span"><i>k</i></span> journeys. If it is impossible for the bus to make <span class="tex-span"><i>k</i></span> journeys, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 &lt; <i>f</i> &lt; <i>a</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>) — the endpoint of the first bus journey, the capacity of the fuel tank of the bus, the point where the gas station is located, and the required number of journeys.</p>

## Output

<p>Print the minimum number of times the bus needs to refuel to make <span class="tex-span"><i>k</i></span> journeys. If it is impossible for the bus to make <span class="tex-span"><i>k</i></span> journeys, print <span class="tex-font-style-tt">-1</span>.</p>

## Samples

```input1
6 9 2 4

```

```output1
4

```






```input2
6 10 2 4

```

```output2
2

```






```input3
6 5 4 3

```

```output3
-1

```




## Note

<p>In the first example the bus needs to refuel during each journey.</p><p>In the second example the bus can pass <span class="tex-span">10</span> units of distance without refueling. So the bus makes the whole first journey, passes <span class="tex-span">4</span> units of the distance of the second journey and arrives at the point with the gas station. Then it can refuel its tank, finish the second journey and pass <span class="tex-span">2</span> units of distance from the third journey. In this case, it will again arrive at the point with the gas station. Further, he can refill the tank up to <span class="tex-span">10</span> liters to finish the third journey and ride all the way of the fourth journey. At the end of the journey the tank will be empty. </p><p>In the third example the bus can not make all <span class="tex-span">3</span> journeys because if it refuels during the second journey, the tanks will contain only <span class="tex-span">5</span> liters of gasoline, but the bus needs to pass <span class="tex-span">8</span> units of distance until next refueling.</p>
