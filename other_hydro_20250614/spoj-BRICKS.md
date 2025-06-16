<p align="justify">
You have n bricks arranged in a line on the table. There is exactly one letter on each of them. Your task is to rearrange those bricks so that letters on them create some specified inscription. While rearanging you can only swap adjacent bricks with specified letters (you are given m pairs (a1,b1),...,(am,bm) and you are only allowed to swap bricks with ai on one of them and bi on the second, for some i=1,..,m). You should check if it is possible to accomplish this - and if it is - calculate minimal needed number of swaps.
</p>
<h3>Input</h3>
<p align="justify">
There is a single integer c on the first line of input. Then c test cases follow: each of them consists of two lines of small letters (a..z) with lengths not exceeding 100000 (descriptions of starting and ending configurations), one integer m in the next line and then m lines with two letters ai,bi in each of them.
</p>
<h3>Output</h3>
<p align="justify">
For each test case you should print -1 if it is not possible to rearrange bricks or the minimal number of swaps if it is possible (if so, output this value modulo 2<sup>32</sup>).
</p>
<h3>Example</h3>
<pre>Input:
4
ab
ba
0
abc
cba
3
ab
cb
ca
cabbbc
cbabbc
1
ab
abba
baab
1
ab

Output:
-1
3
1
2
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>