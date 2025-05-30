<p>You are given the sequence of all K-digit binary numbers:
0, 1,..., 2<sup>K</sup>-1.
You need to fully partition the sequence into M chunks.  Each chunk
must be a consecutive subsequence of
the original sequence.  Let S<sub>i</sub> (1 �� i �� M) be the total
number of 1's in all
numbers in the ith chunk when written in binary, and let S be the
maximum of all S<sub>i</sub>,
i.e. the maximum number of 1's in any chunk.  Your goal is to
minimize S.

</p><h3>Input</h3>
<p>In the first line of input, two numbers, K and M (1 �� K ��
100, 1 �� M �� 100, M �� 2^K), are given,
separated by a single space character.

</p><h3>Output</h3>
<p>In one line of the output, write the minimum S that can be obtained
by some split. Write it without leading zeros. The result is not
guaranteed to fit in a 64-bit integer.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 4

<b>Output:</b>
4
</pre>