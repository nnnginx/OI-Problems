<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/LUCKYNUM/en/">English</a></td> 
<td width="50%"><a href="/problems/LUCKYNUM/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>In some Asian countries, 8 and 6 are considered lucky digits. Any number containing only 8s and 6s is considered lucky number, e.g. 6, 8, 66, 668, 88, 886 бн.
Nguyen is a student who likes mathematics very much. Nguyen likes lucky numbers but only of the form
</p>
<p>
                      S = 8бн86бн6
</p>
<p>
where S has at least one digit and the number of 8s or 6s can be zero. Examples of S are 8, 88, 6, 66, 86, 886, 8866 бн
</p>
<p>
Given a positive integer X (1 &lt; X &lt; 10 000), Nguyen wants to find the smallest lucky number S which has at most 200 digits and is divisible by X.
</p>
<p>
Your task is to write a program to find that number for Nguyen.
</p>
<h3>Input</h3>
<p>
The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.
</p>
<p>
For each data test, there is one single line containing the integer X.
</p>
<h3>Output</h3>
<p>
For each data test, write in one line the smallest lucky number S which is divisible by X. In case there is no such a number which has at most 200 digits, write -1.
</p>
<h3>Example</h3>
<pre><b>Sample Input</b>
4
6
8
43
5	

<b>Sample Output</b>
6
8
86
-1
</pre>