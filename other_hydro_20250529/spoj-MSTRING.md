<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MSTRING/en/">English</a></td> 
<td width="50%"><a href="/problems/MSTRING/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
Substring of some string A is defined as one or more (not necessary succeeding)
elements of the string with maintaining the sequence. 
</p><p>
There are given two strings, string VOKI and string TOKI. Write the program that
will calculate the length of any shortest substring of string VOKI such 
as it is not substring of string TOKI.  
</p><p>
</p><h3>Input</h3>
<p></p><p>
In first line of input file there is string VOKI and in second one is string TOKI. 
The only characters that will occur are lowercase characters of 
English alphabet (¡®a¡¯- ¡®z¡¯). String lengths will be less or equal to 1000. 
</p><p>
Note: input data will be such so there will always be a solution.
</p><p>
</p><h3>Output</h3>
<p></p><p>
In the first line of file you should print the length of wanted substring.
</p><p>
</p><h3>Sample</h3>
<pre>Sample input
 
banana 
anbnaanbaan 
 
Sample output
 
5 
 
(eg. banna) 

Sample input
 
babab 
babba 
 
Sample output
 
3 
 
(eg. aab) 
</pre>