## Description

<div><p>You have a description of a lever as string <span class="tex-span"><i>s</i></span>. We'll represent the string length as record <span class="tex-span">|<i>s</i>|</span>, then the lever looks as a horizontal bar with weights of length <span class="tex-span">|<i>s</i>| - 1</span> with exactly one pivot. We will assume that the bar is a segment on the <span class="tex-span"><i>Ox</i></span> axis between points <span class="tex-span">0</span> and <span class="tex-span">|<i>s</i>| - 1</span>.</p><p>The decoding of the lever description is given below.</p><ul> <li> If the <span class="tex-span"><i>i</i></span>-th character of the string equals "<span class="tex-font-style-tt">^</span>", that means that at coordinate <span class="tex-span"><i>i</i></span> there is the pivot under the bar. </li><li> If the <span class="tex-span"><i>i</i></span>-th character of the string equals "<span class="tex-font-style-tt">=</span>", that means that at coordinate <span class="tex-span"><i>i</i></span> there is nothing lying on the bar. </li><li> If the <span class="tex-span"><i>i</i></span>-th character of the string equals digit <span class="tex-span"><i>c</i></span> (<span class="tex-font-style-tt">1-9</span>), that means that at coordinate <span class="tex-span"><i>i</i></span> there is a weight of mass <span class="tex-span"><i>c</i></span> on the bar. </li></ul><p>Your task is, given the lever description, print if it will be in balance or not. Assume that the bar doesn't weight anything. Assume that the bar initially is in balance then all weights are simultaneously put on it. After that the bar either tilts to the left, or tilts to the right, or is in balance.</p></div><div class="input-specification"><p>The first line contains the lever description as a non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(3 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span>, consisting of digits (<span class="tex-font-style-tt">1-9</span>) and characters "<span class="tex-font-style-tt">^</span>" and "<span class="tex-font-style-tt">=</span>". It is guaranteed that the line contains exactly one character "<span class="tex-font-style-tt">^</span>". It is guaranteed that the pivot of the lever isn't located in any end of the lever bar.</p><p>To solve the problem you may need 64-bit integer numbers. Please, do not forget to use them in your programs.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">left</span>" if the given lever tilts to the left, "<span class="tex-font-style-tt">right</span>" if it tilts to the right and "<span class="tex-font-style-tt">balance</span>", if it is in balance.</p></div>


## Input

<p>The first line contains the lever description as a non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(3 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span>, consisting of digits (<span class="tex-font-style-tt">1-9</span>) and characters "<span class="tex-font-style-tt">^</span>" and "<span class="tex-font-style-tt">=</span>". It is guaranteed that the line contains exactly one character "<span class="tex-font-style-tt">^</span>". It is guaranteed that the pivot of the lever isn't located in any end of the lever bar.</p><p>To solve the problem you may need 64-bit integer numbers. Please, do not forget to use them in your programs.</p>


## Output

<p>Print "<span class="tex-font-style-tt">left</span>" if the given lever tilts to the left, "<span class="tex-font-style-tt">right</span>" if it tilts to the right and "<span class="tex-font-style-tt">balance</span>", if it is in balance.</p>


## Samples

```input1
=^==

```

```output1
balance

```






```input2
9===^==1

```

```output2
left

```






```input3
2==^7==

```

```output3
right

```






```input4
41^52==

```

```output4
balance

```




## Note

<p>As you solve the problem, you may find the following link useful to better understand how a lever functions: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Lever</span>.</p><p>The pictures to the examples:</p><center> <img class="tex-graphics" src="./26740/file/bkxe3pjI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="./26740/file/dz4SpHZu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="./26740/file/rBKBzk51.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="./26740/file/vgJG5sWq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>

