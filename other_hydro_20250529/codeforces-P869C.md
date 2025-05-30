## Description

<div><p><span class="tex-font-style-it">— This is not playing but duty as allies of justice, Nii-chan!</span></p><p><span class="tex-font-style-it">— Not allies but justice itself, Onii-chan!</span></p><p>With hands joined, go everywhere at a speed faster than our thoughts! This time, the Fire Sisters&nbsp;— Karen and Tsukihi&nbsp;— is heading for somewhere they've never reached&nbsp;— water-surrounded islands!</p><p>There are three clusters of islands, conveniently coloured red, blue and purple. The clusters consist of <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> distinct islands respectively.</p><p>Bridges have been built between some (possibly all or none) of the islands. A bridge bidirectionally connects two different islands and has length <span class="tex-span">1</span>. For any two islands of the same colour, either they shouldn't be reached from each other through bridges, or the shortest distance between them is <span class="tex-font-style-bf">at least <span class="tex-span">3</span></span>, apparently in order to prevent oddities from spreading quickly inside a cluster.</p><p>The Fire Sisters are ready for the unknown, but they'd also like to test your courage. And you're here to figure out the number of different ways to build all bridges under the constraints, and give the answer modulo <span class="tex-span">998 244 353</span>. Two ways are considered different if a pair of islands exist, such that there's a bridge between them in one of them, but not in the other.</p></div><div class="input-specification"><p>The first and only line of input contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 5 000</span>)&nbsp;— the number of islands in the red, blue and purple clusters, respectively.</p></div><div class="output-specification"><p>Output one line containing an integer&nbsp;— the number of different ways to build bridges, modulo <span class="tex-span">998 244 353</span>.</p></div>

## Input

<p>The first and only line of input contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 5 000</span>)&nbsp;— the number of islands in the red, blue and purple clusters, respectively.</p>

## Output

<p>Output one line containing an integer&nbsp;— the number of different ways to build bridges, modulo <span class="tex-span">998 244 353</span>.</p>

## Samples

```input1
1 1 1

```

```output1
8

```






```input2
1 2 2

```

```output2
63

```






```input3
1 3 5

```

```output3
3264

```






```input4
6 2 9

```

```output4
813023575

```




## Note

<p>In the first example, there are <span class="tex-span">3</span> bridges that can possibly be built, and no setup of bridges violates the restrictions. Thus the answer is <span class="tex-span">2<sup class="upper-index">3</sup> = 8</span>.</p><p>In the second example, the upper two structures in the figure below are instances of valid ones, while the lower two are invalid due to the blue and purple clusters, respectively.</p><center> <img class="tex-graphics" src="./28813/file/o1m5yzvD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
