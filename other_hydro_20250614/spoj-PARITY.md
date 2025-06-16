<p>You are given n binary strings s<sub>1</sub>,...,s<sub>n</sub>, each of the same
length m.  Along with each s<sub>i</sub> you are given a bit b<sub>i</sub>.  You are
also given some nonnegative integer k and want to know whether there
exists a subset S of {0,1,...,m-1} of size at most k such
that for each i=1,2,...,n, the bit b<sub>i</sub> is the XOR of the bits
of s<sub>i</sub> at the indices in S.  The s<sub>i</sub> are 0-indexed strings.
Recall that the XOR of a set of bits
is 1 if the number of bits equal to 1 is odd, else the XOR is 0
(in particular, the XOR of an empty set of bits is 0).

For example, if s<sub>1</sub> = 1010 and S = {0,3}, then b<sub>1</sub> would be
1 (the first bit of s<sub>1</sub>) XOR'd with 0 (the last bit of s<sub>1</sub>),
which is 1.

Given n, k, and the strings s<sub>1</sub>,...,s<sub>n</sub> and their
corresponding b<sub>i</sub>, find a set S of size at most k which produces
the given b<sub>i</sub>.  You should also detect when no such S exists.

</p><h3>Input</h3>
<p>The first line contains n and k, space-separated (1 �� n ��
64, 0 �� k �� 10).  n lines then follow, where the ith line
contains s<sub>i</sub>, followed by a space, then b<sub>i</sub>.  In a given test case
all strings s<sub>i</sub> are of the same length m (1 �� m �� 50).  k
will not be bigger than m.

</p><h3>Output</h3>
<p>If no set S of size at most k exists producing the given b<sub>i</sub>,
output -1 followed by a newline.  Otherwise, on the first line
output the size of a possible S.  If the size of that S is not
0, on
the second line, output a space-separated list of the indices in S,
followed by a newline.  If there exist multiple valid S to be
output, you can output any one of your choosing.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 1
111 1
001 0
011 1

<b>Output:</b>
1
1
</pre>