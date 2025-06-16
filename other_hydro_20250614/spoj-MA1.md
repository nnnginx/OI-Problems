<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MA1/en/">English</a></td> 
<td width="50%"><a href="/problems/MA1/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
Our country needs to be connected by highways that need to be repaired 
every once in a while. A committee chosen by the government of 
our country tries to continually improve the condition of the main highway 
imaginatively named ¡°A1¡± by finding the first damage that needs to 
be fixed.</p><p> Starting with the first damage the highway is divided into 
segments of the same length. A damage fixing team is 
then being 
sent to each segment containing damage. Since there usually are 
much more damages than teams available, it would be advisable to 
divide the highway into segments of given length in such a way that 
the number of segments containing damages is as small as possible. </p><p>
There are N known damages on the highway, each described by an integer 
representing its distance from the beginning of the highway in 
meters. The length of a segment is M meters (an integer). 
There are no damages within the first M meters. The first segment has 
to start within the first M meters of the highway. If the first segment 
starts at the Kth meter then Lth segment starts at the (K+(L-1)*M)th
meter of the highway. A team can fix all damages occurring within
one segment starting with the first meter of the segment and ending 
with the last meter of that segment. </p><p>
Write a program that will determine the minimal number of damage fixing 
teams needed to fix all damages occurring on the highway ¡°A1¡± and all 
possible beginnings of the first segment. 
 
</p><p>
</p><h3>Input</h3>
<p></p><p>
The first line of the input file contains two whole numbers M and
N separated by a space character, 1 ¡Ü M, N ¡Ü 100 000, where M is a 
length of a segment and N is a number of damages ccurring on the highway. </p><p>
The second line contains N whole numbers separated by a space character
representing the positions of all damages. Each of those numbers is 
greater than M and less than or equal to 2 000 000 000 (two billion). 
The sequence of N numbers given in the second line will always be 
strictly increasing sequence. 
</p><p>
</p><h3>Output</h3>
<p></p><p>
The first line of the output file should contain the minimal number 
of damage fixing teams. </p><p>
The second line should contain all the positions where the first 
segment can begin. These numbers should be separated by a space character 
and they must form a strictly increasing sequence. </p><p>
</p><h3>Sample</h3>
<pre>a1.in 
 
3 5 
4 5 7 8 9 
 
a1.out 
 
2 
1 

a1.in 
 
4 3 
7 14 15 
 
a1.out 
 
2 
1 2 4

a1.in 
 
2 10 
3 4 7 8 12 13 14 15 20 21 
 
a1.out 
 
7 
1 2 
</pre>