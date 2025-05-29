<p>You have been asked to buy a gift for your baby brother, Ike. However, you have noticed that 
Ike has a very particular taste in gifts. He only likes gifts that are configured in his particular 
style. </p>
<p>You have found a shop that sells mobiles. A mobile is a multi-layered decoration that is typically 
hung from the roof. Each mobile consists of a series of horizontal rods connected by vertical wires. 
Each rod has a wire hanging from both ends, which holds either another horizontal rod or a toy. </p>
<p>A sample mobile is shown below: </p>
<img src="/content/john_jones:mobile21.jpg">
<p>To satisfy your brother, you need to find a mobile that can be reconfigured so that: </p>
<p>(i) any two toys are either at the same level (that is, joined to the roof by the same number of 
rods), or di.er by only one level; </p>
<p>(ii) for any two toys that differ by one level, the toy to the left is further down than the toy to 
the right. </p>
<p>Mobiles can be reconfigured by performing swaps. A swap involves taking some rod, unhooking 
whatever is hanging beneath the left and right ends, and reattaching them at opposite ends (that 
is, the right and left ends respectively). This process does not modify the ordering of any rods or 
toys further down. </p>
<p>Since you are training for the Informatics Olympiad, you decide to write a program to test 
whether a given mobile can be reconfigured into a gift that Ike will like! </p>
<p>As an example, consider the mobile illustrated earlier. Ike will not like this mobile. Although 
it satisfies condition (i), it breaks condition (ii) �� the toy at the leftmost end is at a higher level 
than the toys to its right. </p>
<p>However, the mobile can be reconfigured into a mobile that Ike will like. The following swaps 
are required: </p>
<p>1. First, the left and right ends of rod 1 are swapped. This exchanges the positions of rods 2 
and 3, resulting in the following configuration: </p>
<img src="/content/john_jones:mobile22.jpg">
<p>2. Second, and finally, the left and right ends of rod 2 are swapped. This moves rod 4 to the 
left end of rod 2, and the toy to the right end of rod 2. </p>
<img src="/content/john_jones:mobile23.jpg">
<p>It can be seen that this final mobile satisfies Ike's requirements. All toys are at most one level 
apart, and the toys at a lower level are further to the left than the toys at a higher level. </p>
<p>Your task is, given a description of a mobile, to determine the smallest number of swaps required 
to reconfigure it so that Ike will like it (if this is possible). You may assume that the toys can 
never get in each other's way. </p>

<h3>Input </h3>
<p>Multiple test cases, the number of them will be given at the very first line.</p>
<p>For each test case:</p>
<p>The first line of input will contain the single integer n (1 &lt;= n &lt;= 100 000) representing the number 
of rods in the mobile. The rods are numbered 1, 2 , ..., n.</p> 
<p>The following n lines will describe the connections for each rod. Specifically, the ith of these 
lines will describe rod i. Each of these lines will contain two integers <i>l</i> <i>r</i> separated by a single 
space, indicating what is hung beneath the left and right ends of the rod respectively. If a toy is 
hung beneath this rod, the corresponding integer <i>l</i> or <i>r</i> will be -1. Otherwise the integer <i>l</i> or <i>r</i> will be the number of a rod that is hung beneath this rod. </p>

<p>If there are any rods hanging beneath rod i, these rods will have numbers strictly greater than i. Rod 1 is the single rod at the top of the mobile. </p>
<h3>Output </h3>
<p>Output should consist of a single line containing a single integer, giving the smallest number of 
swaps required to reconfigure the mobile according to Ike's constraints. If this is not possible, you 
should output the integer -1. </p>
<h3>Example</h3>
<pre><b>Input:</b>
1
6
2 3 
-1 4 
5 6 
-1 -1 
-1 -1 
-1 -1 

<b>Output:</b>
2
</pre>
<b>Warning: large input/output data,be careful with certain languages</b>