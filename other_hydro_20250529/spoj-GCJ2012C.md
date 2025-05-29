<p>Do you ever become frustrated with television because you keep seeing the same things, recycled over and over again? Well I personally don't care about television, but I do sometimes feel that way about numbers.

</p><p>Let's say a pair of distinct positive integers (n, m) is recycled if you can obtain m by moving some digits from the back of n to the front without changing their order. For example, (12345, 34512) is a recycled pair since you can obtain 34512 by moving 345 from the end of 12345 to the front. Note that n and m must have the same number of digits in order to be a recycled pair. Neither n nor m can have leading zeros.

</p><p>Given integers A and B with the same number of digits and no leading zeros, how many distinct recycled pairs (n, m) are there with A ¡Ü n &lt; m ¡Ü B?

</p><p>Limits<br>
1 ¡Ü T ¡Ü 55<br>
A and B have the same number of digits.<br>
1 ¡Ü A ¡Ü B ¡Ü 2000000.<br>

</p><p>Are we sure about the output to Case #4?<br>
Yes, we're sure about the output to Case #4.

</p><h3>Input</h3>
<p>The first line of the input gives the number of test cases, T. T test cases follow. Each test case consists of a single line containing the integers A and B.

</p><h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is the case number (starting from 1), and y is the number of recycled pairs (n, m) with A ¡Ü n &lt; m ¡Ü B.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
1 9
10 40
100 500
1111 2222

<b>Output:</b>
Case #1: 0
Case #2: 3
Case #3: 156
Case #4: 287
</pre>