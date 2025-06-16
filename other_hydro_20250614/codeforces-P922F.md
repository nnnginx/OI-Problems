## Description

<div><p>Imp is really pleased that you helped him. But it you solve the last problem, his gladness would raise even more.</p><center> <img class="tex-graphics" src="./29039/file/kL0Ag6R4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Let's define <img align="middle" class="tex-formula" src="./29039/file/9x1ZcAmz.png" style="max-width: 100.0%;max-height: 100.0%;"> for some set of integers <img align="middle" class="tex-formula" src="./29039/file/pPdA41Ib.png" style="max-width: 100.0%;max-height: 100.0%;"> as the number of pairs <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> in <img align="middle" class="tex-formula" src="./29039/file/LRNNp5M3.png" style="max-width: 100.0%;max-height: 100.0%;">, such that:<ul> <li> <span class="tex-span"><i>a</i></span> is <span class="tex-font-style-bf">strictly less</span> than <span class="tex-span"><i>b</i></span>; </li><li> <span class="tex-span"><i>a</i></span> <span class="tex-font-style-bf">divides</span> <span class="tex-span"><i>b</i></span> without a remainder. </li></ul><p>You are to find such a set <img align="middle" class="tex-formula" src="./29039/file/tAIs7Dzu.png" style="max-width: 100.0%;max-height: 100.0%;">, which is a subset of <span class="tex-span">{1, 2, ..., <i>n</i>}</span> (the set that contains all positive integers not greater than <span class="tex-span"><i>n</i></span>), that <img align="middle" class="tex-formula" src="./29039/file/ZbpCW0Xo.png" style="max-width: 100.0%;max-height: 100.0%;">. </p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <img align="middle" class="tex-formula" src="./29039/file/HKbC8nCz.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>If there is no answer, print "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">Yes</span>", in the second&nbsp;— an integer <span class="tex-span"><i>m</i></span> that denotes the size of the set <img align="middle" class="tex-formula" src="./29039/file/gT6sHR4C.png" style="max-width: 100.0%;max-height: 100.0%;"> you have found, in the second line print <span class="tex-span"><i>m</i></span> integers&nbsp;— the elements of the set <img align="middle" class="tex-formula" src="./29039/file/sGDQk4a4.png" style="max-width: 100.0%;max-height: 100.0%;">, in any order.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <img align="middle" class="tex-formula" src="./29039/file/HKbC8nCz.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>If there is no answer, print "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">Yes</span>", in the second&nbsp;— an integer <span class="tex-span"><i>m</i></span> that denotes the size of the set <img align="middle" class="tex-formula" src="./29039/file/gT6sHR4C.png" style="max-width: 100.0%;max-height: 100.0%;"> you have found, in the second line print <span class="tex-span"><i>m</i></span> integers&nbsp;— the elements of the set <img align="middle" class="tex-formula" src="./29039/file/sGDQk4a4.png" style="max-width: 100.0%;max-height: 100.0%;">, in any order.</p><p>If there are multiple answers, print any of them.</p>

## Samples

```input1
3 3

```

```output1
No

```






```input2
6 6

```

```output2
Yes
5
1 2 4 5 6
```






```input3
8 3

```

```output3
Yes
4
2 4 5 8

```




## Note

<p>In the second sample, the valid pairs in the output set are <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 4)</span>, <span class="tex-span">(1, 5)</span>, <span class="tex-span">(1, 6)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(2, 6)</span>. Thus, <img align="middle" class="tex-formula" src="./29039/file/0DDSI8GE.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third example, the valid pairs in the output set are <span class="tex-span">(2, 4)</span>, <span class="tex-span">(4, 8)</span>, <span class="tex-span">(2, 8)</span>. Thus, <img align="middle" class="tex-formula" src="./29039/file/uEHsAaaA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
