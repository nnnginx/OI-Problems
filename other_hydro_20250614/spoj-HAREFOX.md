<p>The Antique Comedians of Malidinesia play an interesting comedy
where many animals occur. Because they want their plays to be as true as
possible, a specialist studies the behaviour of various animals.
Recently, he is interested in a binary dynamic ecological
system hares-foxes (SHF). As a part of this project, you are asked to design
and implement intelligent automatic target evaluation simulator
(IATES) for this system. The behaviour of the SHF follows so
called <i>standard model</i>, described by the following set of
difference equations.

</p><p align="Center">
h<sub>y+1</sub> = a.h<sub>y</sub> - b.f<sub>y</sub>
<br>f<sub>y+1</sub> = c.f<sub>y</sub> + d.h<sub>y</sub>

</p><p>where h<sub>y</sub> resp. f<sub>y</sub> represent the difference of the
number of hares resp. foxes in year <sub>y</sub> and the reference count
determined at the beginning of the experiment. The units of h<sub>y</sub>
and f<sub>y</sub> are unknown. Therefore, h<sub>y</sub> and f<sub>y</sub>
are to be treated as real numbers.
Your task is to write a program to determine the long term evolution of SHF.


</p><h3>Input</h3>

<p>The input consists of <var>N</var> cases (equal to about 5000). The first line of the input
contains only positive integer <var>N</var>. Then follow the cases.
Each case consists of six real numbers <var>a, b, c, d,
h<sub>1998</sub></var> and <var>f<sub>1998</sub></var>,
written in this order on three lines, two numbers per line, separated
by one or more spaces. The numbers are given in the classical format,
i.e. optional sign, sequence of digits, optional dot and optional
sequence of digits. The text form of a number
does not exceed 10 characters. Each case is followed by one empty line.


</p><h3>Output</h3>
<p>
For each case, print one of the following sentences:
</p>
<div align="justify"><ul>

<li> '<tt>Ecological balance will develop.</tt>' -
if after sufficiently long time the population of both hares and foxes 
approaches the reference count with an arbitrary a priori given
precision, i.e. <var>lim h<sub>y</sub>=0</var> and <var>lim
f<sub>y</sub>=0</var>.

</li><li>'<tt>Hares will die out while foxes will overgrow.</tt>' -
if after sufficiently long time the population of hares resp. foxes 
falls under resp. exceeds any a priori given threshold, i.e.
<var>lim h<sub>y</sub>=-infinity</var> and
<var>lim f<sub>y</sub>=+infinity</var>.

</li><li>'<tt>Hares will overgrow while foxes will die out.</tt>' -
if after sufficiently long time the population of foxes resp. hares
falls under resp. exceeds any a priori given threshold, i.e.
<var>lim h<sub>y</sub>=+infinity</var> and
<var>lim f<sub>y</sub>=-infinity</var>.

</li><li>'<tt>Both hares and foxes will die out.</tt>' -
if after sufficiently long time the population of both hares and foxes
falls under any a priori given threshold, i.e.
<var>lim h<sub>y</sub>=-infinity</var> and
<var>lim f<sub>y</sub>=-infinity</var>.

</li><li>'<tt>Both hares and foxes will overgrow.</tt>' -
if after sufficiently long time the population of both hares and foxes
exceeds any a priori given threshold, i.e.
<var>lim h<sub>y</sub>=+infinity</var> and
<var>lim f<sub>y</sub>=+infinity</var>.

</li><li>'<tt>Chaos will develop.</tt>' - if none of the above mentioned 
description fits.

</li></ul></div>


<h3>Example</h3>
<pre>Sample input:

2
2 0.5
0.5 0.6
2 3

0.1 1 
2 0.1
1 1

Sample output:

Both hares and foxes will overgrow.
Hares will die out while foxes will overgrow.
</pre>