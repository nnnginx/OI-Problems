<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MSKYCODE/en/">English</a></td> 
<td width="50%"><a href="/problems/MSKYCODE/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
Stancu likes space travels but he is a poor software developer and 
will never be able to buy his own spacecraft. That is why he is 
preparing to steal the spacecraft of Petru. There is only one problem �C 
Petru has locked the spacecraft with a sophisticated cryptosystem 
based on the ID numbers of the stars from the Milky Way Galaxy. For 
breaking the system Stancu has to check each subset of 
four stars 
such that the only common divisor of their numbers is 1. Nasty, isn��t it? </p><p>
Fortunately, Stancu has succeeded to limit the number of the interesting 
stars to N but, any way, the possible subsets of four stars can 
be too many. Help him to find their number and to decide if there is 
a chance to break the system. </p><p>
 
</p><h3>Input</h3>
<p></p><p>
In the input file several test cases are given. For each test case on 
the first line the number N of interesting stars is given (1 �� N �� 10000). </p><p>
The second line of the test case contains the list of ID numbers of 
the interesting stars, separated by spaces. Each ID is a positive integer 
which is no greater than 10000. The input data terminate with the end 
of file.    
</p><p> 
</p><h3>Output</h3>
<p></p><p>
For each test case the program should print one line with  the number 
of subsets with the asked property.
</p><p>
</p><h3>Sample</h3>
<pre>Input :
4  
2 3 4 5 
4 
2 4 6 8 
7 
2 3 4 5 7 6 8 
Ouput: 
1 
0 
34 
</pre>