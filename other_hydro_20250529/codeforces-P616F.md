## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Each string has cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Let's define the function of string <img align="middle" class="tex-formula" src="./27708/file/K9TzQrMh.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>s</i>, <i>i</i></sub></span> is the number of occurrences of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">|<i>s</i>|</span> is the length of the string <span class="tex-span"><i>s</i></span>. Find the maximal value of function <span class="tex-span"><i>f</i>(<i>s</i>)</span> over all strings.</p><p>Note that the string <span class="tex-span"><i>s</i></span> is not necessarily some string from <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of strings in <span class="tex-span"><i>t</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains contains a non-empty string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> contains only lowercase English letters.</p><p>It is guaranteed that the sum of lengths of all strings in <span class="tex-span"><i>t</i></span> is not greater than <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p><p>The last line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">7</sup> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the cost of the <span class="tex-span"><i>i</i></span>-th string.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>a</i></span> — the maximal value of the function <span class="tex-span"><i>f</i>(<i>s</i>)</span> over all strings <span class="tex-span"><i>s</i></span>. Note one more time that the string <span class="tex-span"><i>s</i></span> is not necessarily from <span class="tex-span"><i>t</i></span>.</p></div>


## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of strings in <span class="tex-span"><i>t</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains contains a non-empty string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> contains only lowercase English letters.</p><p>It is guaranteed that the sum of lengths of all strings in <span class="tex-span"><i>t</i></span> is not greater than <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p><p>The last line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">7</sup> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the cost of the <span class="tex-span"><i>i</i></span>-th string.</p>


## Output

<p>Print the only integer <span class="tex-span"><i>a</i></span> — the maximal value of the function <span class="tex-span"><i>f</i>(<i>s</i>)</span> over all strings <span class="tex-span"><i>s</i></span>. Note one more time that the string <span class="tex-span"><i>s</i></span> is not necessarily from <span class="tex-span"><i>t</i></span>.</p>


## Samples

```input1
2
aa
bb
2 1

```

```output1
4

```






```input2
2
aa
ab
2 1

```

```output2
5

```



