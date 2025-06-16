<p align="justify">
There is a large room in the Pyramid called <em>Room-of-No-Return</em>. Its
floor is covered by rectangular tiles of equal size. The name of the room
was chosen because of the very high number of traps and mechanisms in it.
The ACM group has spent several years studying the secret plan of this room.
It has made a clever plan to avoid all the traps. A specially trained
mechanic was sent to deactivate the most feared trap called Shattered Bones.
After deactivating the trap the mechanic had to escape from the room.
It is very important to step on the center of the tiles only; he must
not touch the edges. One wrong step and a large rock 
falls from the ceiling squashing the mechanic like a pancake. After deactivating
the trap, he realized a horrible thing: the ACM plan did not take his
equipment box into consideration. The box must be laid onto the
ground because the mechanic must have both hands free to prevent contact with
other traps. But when the box is laid on the ground, it could touch the line
separating the tiles. And this is the main problem you are to solve.

</p><h3>Input</h3>
<p align="justify">
The input consists of <var>T</var> test cases (T is equal to about 10000). The number of them (<var>T</var>) is given on
the first line of the input file.
Each test case consists of a single line. The line contains exactly four
integer numbers separated by spaces: <var>A</var>, <var>B</var>,
<var>X</var> and <var>Y</var>. <var>A</var> and <var>B</var>indicate the
dimensions of the tiles, <var>X</var> and <var>Y</var> are the dimensions of
the equipment box (<var>1 &lt;= A,B,X,Y &lt;= 50000</var>).

</p><h3>Output</h3>

<p align="justify">Your task is to determine whether it is possible to put the box on 
a&nbsp;single tile -- that is, if the whole box fits on a&nbsp;single tile without
touching its border. If so, you are to print one line with the
sentence "<code>Escape is possible.</code>". Otherwise print the sentence
"<code>Box cannot be dropped.</code>".


</p><h3>Example</h3>

<pre>Sample Input:

2
10 10 8 8
8 8 10 10

Sample output:

Escape is possible.
Box cannot be dropped.
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>