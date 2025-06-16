<p>You are given a sequence of positive integers a<sub>1</sub>, a<sub>2</sub>, . . . , a<sub>n</sub>. We would like to order the numbers from 1 to
n in such a way, that the i-th number is not greater than a<sub>i</sub> (for each i). In other words, we are looking for
a permutation p of numbers from 1 to n, which satisfies: p<sub>i</sub> ≤ a<sub>i</sub> for each 1 ≤ i ≤ n. There is one more problem,
the sequence ai may change over time. . .</p>
<h3>Input</h3>
<p>The first line of standard input contains one integer n (1 ≤ n ≤ 200 000), the number of elements of the a<sub>i</sub>
sequence. In the second line, there is a sequence of n positive integers a<sub>i</sub> (1 ≤ a<sub>i</sub> ≤ n), separated by single
spaces. The third line contains one integer m (0 ≤ m ≤ 500 000), representing the number of modifications
made to the ai sequence. The following m lines describe these modifications. Each description consists of two
integers j<sub>i</sub> and w<sub>i</sub> (1 ≤ j<sub>i</sub>, w<sub>i</sub> ≤ n for 1 ≤ i ≤ m), separated by single spaces and meaning that j<sub>i</sub>-th element
of the sequence becomes w<sub>i</sub>. The operations take place in turns, so the i-th modification is applied to the
sequence altered by (i − 1) previous modifications.</p>
<h3>Output</h3>
<p>Your program should output exactly m + 1 lines to the standard output. Each of those lines should contain
one word TAK (meaning YES) or NIE (meaning NO). The word in the first line should tell if there exists
a permutation p, which satisfies p<sub>i</sub> ≤ a<sub>i</sub> for each i (for the original a<sub>i</sub> sequence), whereas the words from
following lines answer the question whether there exist any (potentially different) permutations that satisfy
the given conditions for the ai sequence after each modification.</p>
<h3>Example</h3>
<p>For the input data:</p>
<pre>5
3 4 3 2 5
2
5 4
1 5
</pre>
<p>the correct result is:</p>
<pre>TAK
NIE
TAK
</pre>
<p>Explanation of the example. For the original ai sequence, the condition is satisfied by permutation
2, 4, 3, 1, 5. After the first modification, the sequence becomes 3, 4, 3, 2, 4 and for this sequence no valid
permutation exists. After the second modification, the sequence is 5, 4, 3, 2, 4. An example of a permutation
p satisfying all constraints for this sequence is 5, 1, 3, 2, 4.</p>