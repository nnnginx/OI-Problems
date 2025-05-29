<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MPOLGRID/en/">English</a></td>
<td width="50%"><a href="/problems/MPOLGRID/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><pre>The ultimate Tantra is said to have been kept in the most distinguished 
temple deep in the sacred forest somewhere in Japan. Paleographers 
finally identified its location, surprisingly a small temple in Hiyoshi
, after years of eager research. The temple has an underground secret 
room built with huge stones. This underground megalith is suspected to be
where the Tantra is enshrined.

The room door is, however, securely locked. Legends tell that the key of
the door lock was an integer, that only highest priests knew. As the sect 
that built the temple decayed down, it is impossible to know the integer
now, and the Agency for Cultural Affairs bans breaking up the door. Fortunately,
a figure of a number of rods that might be used as a clue to guess that secret
number is engraved on the door.

Many distinguished scholars have challenged the riddle, but no one could
have ever succeeded in solving it, until recently a brilliant young 
computer scientist finally deciphered the puzzle. Lengths of the rods are 
multiples of a certain unit length. He found that, to find the secret 
number, all the rods should be placed on a grid of the unit length to 
make one convex polygon. Both ends of each rod must be set on grid points.
Elementary mathematics tells that the polygon's area ought to be an 
integer multiple of the square of the unit length. The area size of the 
polygon with the largest area is the secret number which is needed to 
unlock the door.

For example, if you have five rods whose lengths are 1, 2, 5, 5, and 5,
respectively, you can make essentially only three kinds of polygons, 
shown in Figure 1. Then, you know that the maximum area is 19 

<img src="../../../../../content/simes:MPOLGRID.jpg" border="0">

Convex polygons consisting of five rods of lengths 1, 2, 5, 5, and 5

Your task is to write a program to find the maximum area of convex polygons 
using all the given rods whose ends are on grid points.
<h3>Input </h3>
<pre>The input consists of multiple datasets, followed by a line containing a
single zero which indicates the end of the input. The format of a dataset is as follows.

    n
    r1	r2	¡­	rn

n is an integer which means the number rods and satisfies 3 ¡Ü n ¡Ü 6. 
ri is an integer which means the length of the i-th rod and satisfied 1 ¡Ü ri ¡Ü 300.

Sample Input
3
3 4 5
5
1 2 5 5 5
6
195 221 255 260 265 290
6
130 145 169 185 195 265
3
1 1 2
6
3 3 3 3 3 3
0
</pre>
<h3>Output</h3>
<pre>For each dataset, output a line containing an integer which is the area 
of the largest convex polygon. When there are no possible convex polygons 
for a dataset, output ¡°-1¡±. 

Sample output
6
19
158253
-1
-1
18
</pre>
 </pre>