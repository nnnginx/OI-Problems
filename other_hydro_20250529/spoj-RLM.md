<p>Run-length encoding of a number replaces a run of digits (that is, a sequence of consecutive equivalent digits) with the number of digits followed by the digit itself. For example, 44455 would become 3425 (three fours, two fives). Note that run-length encoding does not necessarily shorten the length of the data: 11 becomes 21, and 42 becomes 1412. If a number has more than nine consecutive digits of the same type, the encoding is done greedily: each run grabs as many digits as it can, so 111111111111111 is encoded as 9161.</p>
<p>Implement an integer arithmetic calculator that takes operands and gives results in run-length format. You should support addition, subtraction, multiplication, and division. You won't have to divide by zero or deal with negative numbers.</p>
<h3>Input/Output</h3>
<p>The input will consist of several test cases, one per line. For each test case, compute the run-length mathematics expression and output the original expression and the result, as shown in the examples. The (decimal) representation of all operands and results will fit in signed 64-bit integers.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
11 + 11
988726 - 978625
12 * 41
1124 / 1112
13 * 33
15 / 16

<strong>Output:</strong>
11 + 11 = 12
988726 - 978625 = 919111
12 * 41 = 42
1124 / 1112 = 1112
13 * 33 = 39
15 / 16 = 10
</pre>