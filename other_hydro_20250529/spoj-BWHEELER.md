<p>
The <b>Burrows-Wheeler transform</b> (<b>BWT</b>, also called <b>block-sorting compression</b>), is an algorithm used in data compression techniques such as bzip2. It was invented by Michael Burrows and David Wheeler.
</p><p>When a character string is transformed by the BWT, none of its characters change value. The transformation permutes the order of the characters. If the original string had several substrings that occurred often, then the transformed string will have several places where a single character is repeated multiple times in a row. This is useful for compression, since it tends to be easy to compress a string that has runs of repeated characters by techniques such as move-to-front transform and run-length encoding.</p>
<p>For example, the string:</p>
<pre>SIX.MIXED.PIXIES.SIFT.SIXTY.PIXIE.DUST.BOXES
</pre>

<p>could be transformed into this string, which is easier to compress because it has many repeated characters:</p>
<pre> TEXYDST.E.IXIXIXXSSMPPS.B..E.S.EUSFXDIIOIIIT
</pre>
<p>
Now the Burrows-Wheeler algorithm works as follows:
</p><ul>
<li> Given an input string <b>S</b>, eg: "abcba".
</li><li> Find all rotations of <b>S</b>. <br>
<pre>eg: "abcba", "bcbaa", "cbaab", "baabc", "aabcb"
</pre>
</li><li> Now sort the strings hence produced.
<pre>eg: "aabcb", "abcba", "baabc", "bcbaa", "cbaab"
</pre>
</li><li> Arrange the strings in a len(S) x len(S) grid.
<pre>aabcb
abcba
baabc
bcbaa
cbaab
</pre>
</li><li> Output the row number (1-based indexing) containing the original input string. Also output the strings formed by characters in the last column.<br>
eg: 2 bacab
</li></ul>
<p></p>
<br>
Now given the output of Burrows-Wheeler, can you recover the orginal string?<br>
<br>
<div align="justify">
<b>Input Format:</b><br>
The input file consists of multiple testcases. <br>
The first line of each testcase contains one integer, <b>R</b>, indicating the row number containing the original input string in the sorted matrix. <br>
The second line of each testcase contains one string, <b>Col</b>, which is the last column of the grid. (1 &lt;= len(Col) &lt;= 1000) <br>
<b>Col</b> contains only lowercase characters. 1 &lt;= <b>R</b> &lt;= len(Col).<br>
Input terminates with a line containing R=0 which must not be processed. <br>
<br>
<b>Output Format:</b><br>
Print the original input string to the burrow wheeler's algorithm.<br>
<br>
<b>Testdata:</b><br>
30 testcases<br>
<b>Sample Input:</b><br>
<pre>2
bacab
3
rwlb
11
baaabaaaabbbaba
0
</pre>

<b>Sample Output:</b><br>
<pre>abcba
rbwl
baaabbbbaaaaaab
</pre>
</div>