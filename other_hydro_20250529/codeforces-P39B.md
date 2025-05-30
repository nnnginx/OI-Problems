## Description

<div><p>Petya works as a PR manager for a successful Berland company BerSoft. He needs to prepare a presentation on the company income growth since <span class="tex-span">2001</span> (the year of its founding) till now. Petya knows that in <span class="tex-span">2001</span> the company income amounted to <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> billion bourles, in <span class="tex-span">2002</span> — to <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> billion, ..., and in the current <span class="tex-span">(2000 + <i>n</i>)</span>-th year — <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> billion bourles. On the base of the information Petya decided to show in his presentation the linear progress history which is in his opinion perfect. According to a graph Petya has already made, in the first year BerSoft company income must amount to <span class="tex-span">1</span> billion bourles, in the second year — <span class="tex-span">2</span> billion bourles etc., each following year the income increases by <span class="tex-span">1</span> billion bourles. Unfortunately, the real numbers are different from the perfect ones. Among the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> can even occur negative ones that are a sign of the company’s losses in some years. That is why Petya wants to ignore some data, in other words, cross some numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from the sequence and leave only some subsequence that has perfect growth.</p><p>Thus Petya has to choose a sequence of years <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span>,so that in the year <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> the company income amounted to <span class="tex-span">1</span> billion bourles, in the year <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — <span class="tex-span">2</span> billion bourles etc., in accordance with the perfect growth dynamics. Help him to choose the longest such sequence.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> determines the income of BerSoft company in the <span class="tex-span">(2000 + <i>i</i>)</span>-th year. The numbers in the line are separated by spaces.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>k</i></span> — the maximum possible length of a perfect sequence. In the next line output the sequence of years <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span>. Separate the numbers by spaces. If the answer is not unique, output any. If no solution exist, output one number <span class="tex-span">0</span>.</p></div>


## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> determines the income of BerSoft company in the <span class="tex-span">(2000 + <i>i</i>)</span>-th year. The numbers in the line are separated by spaces.</p>


## Output

<p>Output <span class="tex-span"><i>k</i></span> — the maximum possible length of a perfect sequence. In the next line output the sequence of years <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span>. Separate the numbers by spaces. If the answer is not unique, output any. If no solution exist, output one number <span class="tex-span">0</span>.</p>


## Samples

```input1
10
-2 1 1 3 2 3 4 -10 -2 5

```

```output1
5
2002 2005 2006 2007 2010

```






```input2
3
-1 -2 -3

```

```output2
0

```



