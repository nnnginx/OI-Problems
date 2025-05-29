<p> Given a sequence of positive integers <var>a</var><sub>1</sub>, <var>a</var><sub>2</sub>, ..., <var>a</var><sub><var>N</var></sub>, and 1 ¡Ü <var>i</var> ¡Ü <var>j</var> ¡Ü <var>N</var>, the partial sum from <br><var>i</var> to <var>j</var> is <var>a</var><sub><var>i</var></sub> + <var>a</var><sub><var>i</var>+1</sub> + ... + <var>a</var><sub><var>j</var></sub>.</p>

<p>In this problem, you will be given such a sequence and two integers <var>P</var> and <var>K</var>. Your task is to find the smallest partial sum modulo <var>P</var> that is at least <var>K</var>.</p>

<p>For example, consider the following sequence of integers:</p>

<pre>12     13     15     11     16     26     11</pre>

<p>Here <var>N</var> = 7. Suppose <var>K</var> = 2 and <var>P</var> = 17. Then, the answer is 2 because 11 + 16  + 26 = 53 and 53 mod 17 is 2. On the other hand, if <var>K</var> = 0 the answer is 0 since 15 + 11 + 16 + 26 = 68 and 68 mod 17 is 0.</p>

<p>You may assume 1 ¡Ü <var>N</var> ¡Ü 100000.</p>

<h3>Input</h3>
<p>The first line of the input contains the number of test cases, <var>T</var>.</p>
<p>Each test case begins with a line containing three integers, <var>N</var>, <var>K</var> and <var>P</var>. This is followed by the values of <var>a</var><sub>1</sub>, <var>a</var><sub>2</sub>, ..., <var>a</var><sub><var>N</var></sub>, one per line.</p>

<h3>Output</h3>
<p>Output one line per test case, containing the smallest partial sum modulo <var>P</var> that is at least <var>K</var>, as described above.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
7 2 17
12
13
15
11
16
26
11

<b>Output:</b>
2
</pre>

<b>Warning: large Input/Output data, be careful with certain languages</b>