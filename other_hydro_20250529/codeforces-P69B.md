## Description

<div><p>In Chelyabinsk lives a much respected businessman Nikita with a strange nickname "Boss". Once Nikita decided to go with his friend Alex to the Summer Biathlon World Cup. Nikita, as a very important person, received a token which allows to place bets on each section no more than on one competitor.</p><p>To begin with friends learned the rules: in the race there are <span class="tex-span"><i>n</i></span> sections of equal length and <span class="tex-span"><i>m</i></span> participants. The participants numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. About each participant the following is known:</p><ul><li> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — the number of the starting section, </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the number of the finishing section (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>),</li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the time a biathlete needs to complete an section of the path,</li><li> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the profit in roubles. If the <span class="tex-span"><i>i</i></span>-th sportsman wins on one of the sections, the profit will be given to the man who had placed a bet on that sportsman.</li></ul> <p>The <span class="tex-span"><i>i</i></span>-th biathlete passes the sections from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> inclusive. The competitor runs the whole way in <span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub> + 1)·<i>t</i><sub class="lower-index"><i>i</i></sub></span> time units. It takes him exactly <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> time units to pass each section. In case of the athlete's victory on <span class="tex-span"><i>k</i></span> sections the man who has betted on him receives <span class="tex-span"><i>k</i>·<i>c</i><sub class="lower-index"><i>i</i></sub></span> roubles.</p><p>In each section the winner is determined <span class="tex-font-style-bf">independently</span> as follows: if there is at least one biathlete running this in this section, then among all of them the winner is the one who has ran this section in minimum time (spent minimum time passing this section). In case of equality of times the athlete with the smaller index number wins. If there are no participants in this section, then the winner in this section in not determined. We have to say that in the summer biathlon all the participants are moving at a constant speed.</p><p>We should also add that Nikita can bet on each section and on any contestant running in this section.</p><p>Help the friends find the maximum possible profit.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>). Then follow <span class="tex-span"><i>m</i></span> lines, each containing 4 integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print a single integer, the maximal profit in roubles that the friends can get. In each of <span class="tex-span"><i>n</i></span> sections it is not allowed to place bets on more than one sportsman.</p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>). Then follow <span class="tex-span"><i>m</i></span> lines, each containing 4 integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>


## Output

<p>Print a single integer, the maximal profit in roubles that the friends can get. In each of <span class="tex-span"><i>n</i></span> sections it is not allowed to place bets on more than one sportsman.</p>


## Samples

```input1
4 4
1 4 20 5
1 3 21 10
3 3 4 30
3 4 4 20

```

```output1
60
```






```input2
8 4
1 5 24 10
2 4 6 15
4 6 30 50
6 7 4 20

```

```output2
105
```




## Note

<p>In the first test the optimal bet is: in the 1-2 sections on biathlete 1, in section 3 on biathlete 3, in section 4 on biathlete 4. Total: profit of 5 rubles for 1 section, the profit of 5 rubles for 2 section, profit of 30 rubles for a 3 section, profit of 20 rubles for 4 section. Total profit 60 rubles.</p><p>In the second test the optimal bet is: on 1 and 5 sections on biathlete 1, in the 2-4 sections on biathlete 2, in the 6-7 sections on athlete 4. There is no winner in the 8 section. Total: profit of 10 rubles for 1 section, the profit of 15 rubles for 2,3,4 section, profit of 10 rubles for a 5 section, profit of 20 rubles for 6, 7 section. Total profit 105 rubles.</p>

