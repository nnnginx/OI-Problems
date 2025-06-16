<p>
You are to find all pairs of integers such that their sum is equal to the given integer number N and the second number results from the first one by striking out one of its digits. The first integer always has at least two digits and starts with a non-zero digit. The second integer always has one digit less than the first integer and may start with a zero digit.
</p><h3>Input</h3>
<p>
The first line of the input file is the integer number t ( 1 ¡Ü t ¡Ü 20 ), the number of test cases. Then t lines follow, each test case in one line; the line consists of a single integer N (10 ¡Ü N ¡Ü 10^9).
</p><h3>Output</h3>
<p>
For each test case: </p><p>
On the first line write the total number of different pairs of integers that satisfy the problem statement. On the following lines write all those pairs. Write one pair on a line in ascending order of the first integer in the pair. Each pair must be written in the following format</p><p>

</p><p>X + Y = N</p><p>

Here X, Y, and N, must be replaced with the corresponding integer numbers. There should be exactly one space on both sides of '+' and '=' characters.


</p><h3>Example</h3>

<pre><b>Input:</b>
2
302
11

<b>Output:</b>
5
251 + 51 = 302
275 + 27 = 302
276 + 26 = 302
281 + 21 = 302
301 + 01 = 302
1
10 + 1 = 11
</pre>