<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/PRETTYP/en/">English</a></td> 
<td width="50%"><a href="/problems/PRETTYP/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>
An IT company decided to publish an internal newsletter describing the projects that have been successfully completed. Each department submits a text paragraph that will be printed in a corresponding designated box of the newsletter. Let¡¯s assume that the paragraph contains only characters a...z and spaces (ASCII code is 32) in several lines, and a word is defined to be the longest sequence of non-space characters on a line.
</p>
<p>The printing has to satisfy the following rules:</p>
<ul>
<li>Text will be printed in a fixed-width font (meaning that every character occupies a fixed size width) from left to right and going down to the next line at the end of every line.</li>
<li>The number of printed characters in every line must be the same.</li>
<li>Words are printed in the box in the same order as they appear in the given paragraph. A word cannot be split or printed on more than one line. </li>
<li>Consecutive words on the same line are separated by exactly one space. </li>
<li>Every line contains only words from the original paragraph and spaces.</li>
<li>Any line that starts with a space must contain only spaces. </li>
</ul>
<p>
The newsletter editor wants to formally assess the prettiness level of a paragraph printing by defining the unbalance of it as the sum of the cubes of the number of space characters at the end of each line including lines containing only spaces. The smaller the unbalance, the prettier the paragraph printing is.
</p>
<p>
Consider the following example where the paragraph is printed in a box with three lines and each line has a 20-characters width in two ways:
</p>
<table border="1">
<tbody><tr>
<td>
<pre>aaa bbbbbbbbb c dddd
eeeeeee ffffff
ggggggggg		
</pre>
</td>
<td>
<pre>aaa bbbbbbbbb      
c dddd eeeeeee       
ffffff ggggggggg
</pre>
</td>
</tr>
</tbody></table>

<p>
In this example, the unbalance of the paragraph printing on the left is 0^3 + 6^3 + 11^3 = 1547 while the unbalance of the paragraph printing on the right is 7^3 + 6^3 + 4^3 = 623. The paragraph printing on the right is considered prettier.
</p>
<p>
Given a text paragraph and a box to be printed, your task is to write a program to find the prettiest printing that has the smallest unbalance. 
</p>
<h3>Input</h3>
<p>
The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.
</p>
<p>
For each data set, the first line contains an integer L (0 &lt; L ¡Ü 100) representing the number of lines in the designated box. The second line contains an integer W (0 &lt; W ¡Ü 1000) representing the number of characters width of the box. The remaining lines contain the paragraph with no more than 1000 words ended with a blank line. 
</p>

<h3>Output</h3>
<p>
For each data test, write on one line the corresponding unbalance of the prettiest paragraph printing in the designated box. Write -1 in case there does not exist any way to print the paragraph in the designated box.
</p>
<h3>Example</h3>
<pre><b>Sample Input</b>
3
3
20
aaa bbbbbbbbb 
c dddd
eeeeeee ffffff
ggggggggg

2
5
abcde abcde

2
5
abcde abcde 
a

<b>Sample Output</b>
623
0
-1
</pre>