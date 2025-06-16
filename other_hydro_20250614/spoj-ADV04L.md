<p>If you are travelling a lot you could have met the following problem: different countries use different measurement systems. Notably there are two major measurement systems for distances: metric and imperial. Metric system exploits kilometers while miles are used in the imperial system. It is known that one mile is approximately 1.609 kilometers. By interesting coincidence this is close enough to the value of the golden ration which is about 1.618. On this basis there is an interesting way of converting miles to kilometeres. Let's look into Fibonacci sequence: <i>F</i><sub>1</sub> = <i>F</i><sub>2</sub> = 1, <i>F</i><sub><i>n</i></sub> = <i>F</i><sub><i>n</i>−1</sub> + <i>F</i><sub><i>n</i>−2</sub>, для <i>n</i> &gt; 2. The ratio of two successive Fibonacci numbers <i>F</i><sub><i>n</i>+1</sub>/<i>F</i><sub><i>n</i></sub> tends to golden ration as <i>n</i> tends to infinity. So you can partition the amount of miles you have into Fibonacci numbers, and you should use as large Fibonacci numbers as possible, then for each element in the partition you should go to the next Fibonacci number and sum up the elements again. That way you will get the approximate amount of kilometers. For example, 40 ⇒ 34 + 5 + 1 ⇒ 55 + 8 + 2 ⇒ 65. That means that 40&nbsp;miles is approximately 65&nbsp;kilometers (more precise value is 64,37 kilometers). Write a program that implements this method.

</p><h3>Input</h3>
<p>The first line of input contains number t – the amount of test cases. The description of t test cases follows. Each test consists of a single integer m - the amount of miles.

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 10000<br>
1 &lt;= m &lt;= 10^15

</p><h3>Output</h3>
<p>For each test case output the amount of kilometers calculated using the method given in the statement.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
1
7
40
128

<b>Output:</b>
2
11
65
207

</pre>