## Description

<div><p>A function <img align="middle" class="tex-formula" src="./27636/file/P3XLkU9b.png" style="max-width: 100.0%;max-height: 100.0%;"> is called Lipschitz continuous if there is a real constant <span class="tex-span"><i>K</i></span> such that the inequality <span class="tex-span">|<i>f</i>(<i>x</i>) - <i>f</i>(<i>y</i>)| ≤ <i>K</i>·|<i>x</i> - <i>y</i>|</span> holds for all <img align="middle" class="tex-formula" src="./27636/file/H0vsWpbC.png" style="max-width: 100.0%;max-height: 100.0%;">. We'll deal with a more... discrete version of this term.</p><p>For an array <img align="middle" class="tex-formula" src="./27636/file/Ry8cpjcg.png" style="max-width: 100.0%;max-height: 100.0%;">, we define it's Lipschitz constant <img align="middle" class="tex-formula" src="./27636/file/Swhv2Snd.png" style="max-width: 100.0%;max-height: 100.0%;"> as follows:</p><ul> <li> if <span class="tex-span"><i>n</i> &lt; 2</span>, <img align="middle" class="tex-formula" src="./27636/file/V3F3s82C.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> if <span class="tex-span"><i>n</i> ≥ 2</span>, <img align="middle" class="tex-formula" src="./27636/file/xwkg0MK7.png" style="max-width: 100.0%;max-height: 100.0%;"> over all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span> </li></ul><p>In other words, <img align="middle" class="tex-formula" src="./27636/file/uk7luDls.png" style="max-width: 100.0%;max-height: 100.0%;"> is the smallest non-negative integer such that <span class="tex-span">|<i>h</i>[<i>i</i>] - <i>h</i>[<i>j</i>]| ≤ <i>L</i>·|<i>i</i> - <i>j</i>|</span> holds for all <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>.</p><p>You are given an array <img align="middle" class="tex-formula" src="./27636/file/4gljqHVG.png" style="max-width: 100.0%;max-height: 100.0%;"> of size <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> queries of the form <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. For each query, consider the subarray <img align="middle" class="tex-formula" src="./27636/file/w1xjiuBa.png" style="max-width: 100.0%;max-height: 100.0%;">; determine the sum of Lipschitz constants of <span class="tex-font-style-bf">all subarrays</span> of <img align="middle" class="tex-formula" src="./27636/file/QUuVhhVn.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 100</span>)&nbsp;— the number of elements in array <img align="middle" class="tex-formula" src="./27636/file/xC9CDxcn.png" style="max-width: 100.0%;max-height: 100.0%;"> and the number of queries respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <img align="middle" class="tex-formula" src="./27636/file/xEcD1sKs.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="./27636/file/bqjqtpQN.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The following <span class="tex-span"><i>q</i></span> lines describe queries. The <span class="tex-span"><i>i</i></span>-th of those lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the answers to all queries in the order in which they are given in the input. For the <span class="tex-span"><i>i</i></span>-th query, print one line containing a single integer&nbsp;— the sum of Lipschitz constants of all subarrays of <img align="middle" class="tex-formula" src="./27636/file/klmNy7j5.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>


## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 100</span>)&nbsp;— the number of elements in array <img align="middle" class="tex-formula" src="./27636/file/xC9CDxcn.png" style="max-width: 100.0%;max-height: 100.0%;"> and the number of queries respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <img align="middle" class="tex-formula" src="./27636/file/xEcD1sKs.png" style="max-width: 100.0%;max-height: 100.0%;"> (<img align="middle" class="tex-formula" src="./27636/file/bqjqtpQN.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The following <span class="tex-span"><i>q</i></span> lines describe queries. The <span class="tex-span"><i>i</i></span>-th of those lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>


## Output

<p>Print the answers to all queries in the order in which they are given in the input. For the <span class="tex-span"><i>i</i></span>-th query, print one line containing a single integer&nbsp;— the sum of Lipschitz constants of all subarrays of <img align="middle" class="tex-formula" src="./27636/file/klmNy7j5.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>


## Samples

```input1
10 4
1 5 2 9 1 3 4 2 1 7
2 4
3 8
7 10
1 9

```

```output1
17
82
23
210

```






```input2
7 6
5 7 7 4 6 6 2
1 2
2 3
2 6
1 7
4 7
3 5

```

```output2
2
0
22
59
16
8

```




## Note

<p>In the first query of the first sample, the Lipschitz constants of subarrays of <img align="middle" class="tex-formula" src="./27636/file/ei5HLk6S.png" style="max-width: 100.0%;max-height: 100.0%;"> with length at least <span class="tex-span">2</span> are:</p><ul> <li> <img align="middle" class="tex-formula" src="./27636/file/A4zH9SwR.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="./27636/file/kyS3RhD5.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="./27636/file/50DIAKpQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul><p>The answer to the query is their sum.</p>

