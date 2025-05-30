## Description

<div><p>Polycarpus likes giving presents to Paraskevi. He has bought two chocolate bars, each of them has the shape of a segmented rectangle. The first bar is <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> × <i>b</i><sub class="lower-index">1</sub></span> segments large and the second one is <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> × <i>b</i><sub class="lower-index">2</sub></span> segments large.</p><p>Polycarpus wants to give Paraskevi one of the bars at the lunch break and eat the other one himself. Besides, he wants to show that Polycarpus's mind and Paraskevi's beauty are equally matched, so the two bars must have the same number of squares.</p><p>To make the bars have the same number of squares, Polycarpus eats a little piece of chocolate each minute. Each minute he does the following:</p><ul> <li> he either breaks one bar exactly in half (vertically <span class="tex-font-style-bf">or</span> horizontally) and <span class="tex-font-style-it">eats exactly a half</span> of the bar, </li><li> or he chips of exactly one third of a bar (vertically or horizontally) and <span class="tex-font-style-it">eats exactly a third</span> of the bar. </li></ul><p>In the first case he is left with a <span class="tex-font-style-it">half</span>, of the bar and in the second case he is left with <span class="tex-font-style-it">two thirds</span> of the bar.</p><p>Both variants aren't always possible, and sometimes Polycarpus cannot chip off a half nor a third. For example, if the bar is <span class="tex-span">16 × 23</span>, then Polycarpus can chip off a half, but not a third. If the bar is <span class="tex-span">20 × 18</span>, then Polycarpus can chip off both a half and a third. If the bar is <span class="tex-span">5 × 7</span>, then Polycarpus cannot chip off a half nor a third.</p><p>What is the minimum number of minutes Polycarpus needs to make two bars consist of the same number of squares? Find not only the required minimum number of minutes, but also the possible sizes of the bars after the process.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the initial sizes of the first chocolate bar. The second line of the input contains integers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the initial sizes of the second bar.</p><p>You can use the data of type <span class="tex-font-style-tt">int64</span> (in Pascal), <span class="tex-font-style-tt">long long</span> (in С++), <span class="tex-font-style-tt">long</span> (in Java) to process large integers (exceeding <span class="tex-span">2<sup class="upper-index">31</sup> - 1</span>).</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>m</i></span> — the sought minimum number of minutes. In the second and third line print the possible sizes of the bars after they are leveled in <span class="tex-span"><i>m</i></span> minutes. Print the sizes using the format identical to the input format. Print the sizes (the numbers in the printed pairs) in any order. The second line must correspond to the first bar and the third line must correspond to the second bar. If there are multiple solutions, print any of them.</p><p>If there is no solution, print a single line with integer <span class="tex-font-style-tt">-1</span>.</p></div>


## Input

<p>The first line of the input contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the initial sizes of the first chocolate bar. The second line of the input contains integers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the initial sizes of the second bar.</p><p>You can use the data of type <span class="tex-font-style-tt">int64</span> (in Pascal), <span class="tex-font-style-tt">long long</span> (in С++), <span class="tex-font-style-tt">long</span> (in Java) to process large integers (exceeding <span class="tex-span">2<sup class="upper-index">31</sup> - 1</span>).</p>


## Output

<p>In the first line print <span class="tex-span"><i>m</i></span> — the sought minimum number of minutes. In the second and third line print the possible sizes of the bars after they are leveled in <span class="tex-span"><i>m</i></span> minutes. Print the sizes using the format identical to the input format. Print the sizes (the numbers in the printed pairs) in any order. The second line must correspond to the first bar and the third line must correspond to the second bar. If there are multiple solutions, print any of them.</p><p>If there is no solution, print a single line with integer <span class="tex-font-style-tt">-1</span>.</p>


## Samples

```input1
2 6
2 3

```

```output1
1
1 6
2 3

```






```input2
36 5
10 16

```

```output2
3
16 5
5 16

```






```input3
3 5
2 1

```

```output3
-1

```



