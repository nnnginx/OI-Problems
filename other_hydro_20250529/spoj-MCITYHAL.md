<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MCITYHAL/en/">English</a></td> 
<td width="50%"><a href="/problems/MCITYHAL/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<pre>Because of its age, the City Hall has suffered damage to one of its walls. 
A matrix with M rows and N columns represents the encoded image of that wall, 
where 1 represents an intact wall and 0 represents a damaged wall (like in Figure-1). 
 
1110000111
1100001111
1000000011
1111101111
1110000111 
 
Figure-1 
 
To repair the wall, the workers will place some blocks vertically into 
the damaged area. They can use blocks with a fixed width of 1 and different 
heights of {1,2, ..., M}.  
 
For a given image of the City Hall¡¯s wall, your task is to determine how
many blocks of different heights are needed to fill in the damaged area
of the wall, and to use the least amount of blocks.
</pre>
 
<h3>Input</h3>
<pre>There is only one test case. The case starts with a line containing two 
integers M and N (1 &lt;= M, N &lt;= 200). Each of the following M lines contains
a string with length of N, which consists of ¡°1¡±s 
and/or ¡°0¡±s. These M lines
represent the wall. 

Sample Input
5 10 
1110000111
1100001111
1000000011
1111101111
1110000111
</pre>

<h3>Output</h3>
<pre> 
You should output how many blocks of different heights are needed. 
Use separate lines of the following format: 
 
k Ck 
 
where k ¡Ê {1,2, ..., M} means the height of the block, and Ck means 
the amount of blocks of height k that are needed. You should not output
the lines where Ck = 0. The order of lines is in the 
ascending order of k. 

Sample output
1 7 
2 1 
3 2 
5 1 
</pre>