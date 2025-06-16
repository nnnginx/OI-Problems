<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MSAFE/en/">English</a></td> 
<td width="50%"><a href="/problems/MSAFE/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>
Mirko has decided to rob mini-safe owned by his son so that he could
take away some football stickers which are missing in his big sticker 
collection. </p><p>
Lock on the safe consists of N equal discs, each of them being divided
in 10,000,000 equal segments numbered from 1 to 10,000,000 
clockwise. In the begining, segments on discs having the same number 
are placed one above (beneath) the other. Discs are layed one on the 
other such that the segments are overlaping and each disc is missing 
exactly one segment that is called hole. 
In order to unlock the lock, all holes must be one above (beneath) the other. 
In  one second, Mirko can turn one disc in  one direction (clockwise or 
counterclockwise) for  one segment. </p><p>
Write a program which will find the minimal time that Mirko needs to
open the safe.</p>
 
<h3>Input</h3>
<p>
The first line of the input file contains an integer N, 2 ¡Ü N ¡Ü 100,000, 
the number of discs. </p><p>
The next N lines contain data describing the initial positions of 
the holes on each disc.  
The (i + 1)-th line contains an integer Pi, 1 ¡Ü Pi
 ¡Ü 10000000, 
the initial position of the hole on the i-th disc. 
</p>
<h3>Output</h3>
<p>
The first and only line of the output file should contain the minimal time 
(in seconds). 
Note: take care of the size of that number. </p>


<h3>Sample</h3>
<pre>safe.in 
 
3 
5 
17 
7 
 
safe.out 
 
12 

safe.in 
 
4 
9999999 
7 
16 
9999995 
 
safe.out 
 
29

safe.in 
 
4 
1 
2500001 
5000000 
7500002 
 
safe.out 
 
9999998 

</pre>