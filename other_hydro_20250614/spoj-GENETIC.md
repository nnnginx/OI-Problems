<p>

The connections between mathematics and biology are complicated.
Most of the time they do not run along nice-looking links that merrily join at first glance, but they are abstract and not always easily established.

</p><p>

Lake Vostok - about 14000 square kilometers large, up to 650 meters deep, and covered by 3743 meters of ice - was recently discovered on the Antarctic continent.
The lake remained under conditions of high pressure and no sunlight for several millions of years.
It is believed that ordinary life has evolved to a more efficient form using a genetic code composed of only three bases (the current state of ignorance proclaims the four bases adenine, cytosine, guanine, and thymine).
Until reasonable names are found, the three bases will be abbreviated as <code>N</code>, <code>O</code>, and <code>P</code>.


</p><p>

Moreover, the genome is single-stranded and directed, i.e., we may see it as a sequence over the alphabet <code>{N,O,P}</code>.
Unless risking instability, it is necessary that the genome is a Thue-sequence, due to the Norwegian mathematician A. Thue (1863-1922).
Define a subsegment of a sequence to be a connected subsequence, and call two subsegments adjacent if one follows immediately after the other in the sequence.
A Thue-sequence is a sequence where no adjacent subsegments are equal.
For example, <code>NOPNO</code> is and <code>NOPNPNO</code> is not a Thue-sequence, so that the first may be a genome whereas the second may not.

</p><p>

To be able to simulate experiments with the new genomes, you are asked to generate genomes of certain lengths.

</p><h3>Input Specification</h3><p>

The input contains several test cases.
Each test case consists of an integer <code>n</code>.
You may assume that <code>1&lt;=n&lt;=5000</code>.
The last test case is followed by a zero.

</p><h3>Output Specification</h3><p>

For each test case specified by <code>n</code> output on a single line any genome of length <code>n</code>.
If no genome of length <code>n</code> exists, output a blank line instead.


</p><h3>Sample Input</h3><p>

</p><pre>1
2
10
20
0
</pre>

<h3>Sample Output</h3><p>

</p><pre>N
NO
NONPNOPNPO
NONPNOPNPONOPNONPNOP
</pre>