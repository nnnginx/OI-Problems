## Description

<div><p>Heidi is now just one code away from breaking the encryption of the Death Star plans. The screen that should be presenting her with the description of the next code looks almost like the previous one, though who would have thought that the evil Empire engineers would fill this small screen with several million digits! It is just ridiculous to think that anyone would read them all...</p><p>Heidi is once again given a sequence <span class="tex-span"><i>A</i></span> and two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span>. She needs to find out what the encryption key <span class="tex-span"><i>S</i></span> is.</p><p>Let <span class="tex-span"><i>X</i></span> be a sequence of integers, and <span class="tex-span"><i>p</i></span> a positive integer. We define the <span class="tex-font-style-underline">score</span> of <span class="tex-span"><i>X</i></span> to be the sum of the elements of <span class="tex-span"><i>X</i></span> modulo <span class="tex-span"><i>p</i></span>.</p><p>Heidi is given a sequence <span class="tex-span"><i>A</i></span> that consists of <span class="tex-span"><i>N</i></span> integers, and also given integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span>. Her goal is to split <span class="tex-span"><i>A</i></span> into <span class="tex-span"><i>k</i></span> parts such that: </p><ul> <li> Each part contains at least <span class="tex-span">1</span> element of <span class="tex-span"><i>A</i></span>, and each part consists of contiguous elements of <span class="tex-span"><i>A</i></span>. </li><li> No two parts overlap. </li><li> The total sum <span class="tex-span"><i>S</i></span> of the scores of those parts is <span class="tex-font-style-bf">minimized</span> (not maximized!). </li></ul><p>Output the sum <span class="tex-span"><i>S</i></span>, which is the encryption code.</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers <span class="tex-span"><i>N</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span"><i>k</i> ≤ <i>N</i> ≤ 500 000</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 100</span>) – the number of elements in <span class="tex-span"><i>A</i></span>, the number of parts <span class="tex-span"><i>A</i></span> should be split into, and the modulo for computing scores, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> space-separated integers that are the elements of <span class="tex-span"><i>A</i></span>. Each integer is from the interval <span class="tex-span">[1, 1 000 000]</span>.</p></div><div class="output-specification"><p>Output the number <span class="tex-span"><i>S</i></span> as described in the problem statement.</p></div>

## Input

<p>The first line of the input contains three space-separated integers <span class="tex-span"><i>N</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span"><i>k</i> ≤ <i>N</i> ≤ 500 000</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 100</span>) – the number of elements in <span class="tex-span"><i>A</i></span>, the number of parts <span class="tex-span"><i>A</i></span> should be split into, and the modulo for computing scores, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> space-separated integers that are the elements of <span class="tex-span"><i>A</i></span>. Each integer is from the interval <span class="tex-span">[1, 1 000 000]</span>.</p>

## Output

<p>Output the number <span class="tex-span"><i>S</i></span> as described in the problem statement.</p>

## Samples

```input1
4 3 10
3 4 7 2

```

```output1
6

```






```input2
10 5 12
16 3 24 13 9 8 7 5 12 12

```

```output2
13

```




## Note

<p>In the first example, if the input sequence is split as <span class="tex-span">(3)</span>, <span class="tex-span">(4, 7)</span>, <span class="tex-span">(2)</span>, the total score would be <img align="middle" class="tex-formula" src="./29176/file/x6gjGa9S.png" style="max-width: 100.0%;max-height: 100.0%;">. It is easy to see that this score is the smallest possible.</p><p>In the second example, one possible way to obtain score <span class="tex-span">13</span> is to make the following split: <span class="tex-span">(16, 3)</span>, <span class="tex-span">(24)</span>, <span class="tex-span">(13)</span>, <span class="tex-span">(9, 8)</span>, <span class="tex-span">(7, 5, 12, 12)</span>.</p>
