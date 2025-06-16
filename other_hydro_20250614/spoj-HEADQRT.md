<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/HEADQRT/en/">English</a></td>
<td width="50%"><a href="/problems/HEADQRT/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Microhoo and Googloo are two competing IT companies from the same city. Each company has offices scattered across the city. To protect their critical information from each other, both companies have agreed to locate their headquarters as far from each other as possible.</p>
<p>Given the locations of Microhoo and Googloo existing offices, your task is to write a program to help the two companies to select their headquarters from existing offices so that the distance between their headquarters is longest.</p>
<h3>Input</h3>
<p>The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.</p>
<p>For each data set, the first line contains the integer n (2 ¡Ü n ¡Ü 30000) representing the total number of offices for both companies. The ith line of the next n line contains three integers xi, yi, ci (0 ¡Ü |xi|, |yi| ¡Ü 10<sup>8</sup>, 0 ¡Ü ci ¡Ü 1) separated by space, where (xi, yi) is the coordinate of the ith office and it is Microhoo¡¯s office if ci = 0 and Googloo¡¯s if ci = 1.</p>
<p>It is guaranteed that each company has at least one office.</p>
<h3>Output</h3>
<p>For each data test, write in one line the integer part of the longest distance between Microhoo¡¯s and Googloo¡¯s headquarters.</p>
<h3>Example</h3>
<pre><strong>Sample Input</strong>
2
2
0 0 0
3 -2 1
5
1 5 1 
-5 2 0
3 7 1
6 -2 0 
5 1 0

<strong>Sample Output</strong>
3
9
</pre>
<p> </p>