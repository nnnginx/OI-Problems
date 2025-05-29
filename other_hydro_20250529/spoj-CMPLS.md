<p>

You probably know those quizzes in Sunday magazines: given the sequence 1, 2,
3, 4, 5, what is the next number? Sometimes it is very easy to answer,
sometimes it could be pretty hard. Because these "sequence problems" are very
popular, ACM wants to implement them into the "Free Time" section of their
new WAP portal.

</p><p>
ACM programmers have noticed that some of the quizzes can be solved by
describing the sequence by polynomials. For example, the sequence 1, 2, 3, 4, 5
can be easily understood as a&nbsp;trivial polynomial. The next number is 6. But even
more complex sequences, like 1, 2, 4, 7, 11, can be described by a&nbsp;polynomial.
In this case, 
1/2.<var>n</var><sup>2</sup>-1/2.<var>n</var>+1 can be used. Note that even
if the members of the sequence are integers, polynomial coefficients may be any
real numbers.

</p><p>
Polynomial is an&nbsp;expression in the following form:
<br></p><p></p>
<div align="CENTER">
<var>P</var>(<var>n</var>) = <var>a</var><sub><var>D</var></sub>.<var>n</var><sup><var>D</var></sup>+<var>a</var><sub><var>D</var>-1</sub>.<var>n</var><sup><var>D</var>-1</sup>+...+<var>a</var><sub>1</sub>.<var>n</var>+<var>a</var><sub>0</sub>

</div>
<br clear="ALL">
<p>
If <var>a</var><sub><var>D</var></sub> &lt;&gt; 0, the number <var>D</var> is called a&nbsp;<em>degree</em> of the polynomial. Note
that constant function <var>P</var>(<var>n</var>) = <var>C</var> can be considered as polynomial of degree 0, and
the zero function <var>P</var>(<var>n</var>) = 0 is usually defined to have degree -1.
</p>

<p>
</p><h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 5000). It stands
for the number of test cases to follow. Each test case consists of two
lines. First line of each test case contains two integer numbers <var>S</var> and
<var>C</var> separated by a&nbsp;single space, 
1 &lt;= <var>S</var> &lt; 100, 
1 &lt;= <var>C</var> &lt; 100,

(<var>S</var>+<var>C</var>) &lt;= 100. The first number, <var>S</var>, stands for the length of the given
sequence, the second number, <var>C</var> is the amount of numbers you are to find to
complete the sequence.


</p><p>
The second line of each test case contains <var>S</var> integer numbers

<var>X</var><sub>1</sub>, <var>X</var><sub>2</sub>, ... <var>X</var><sub><var>S</var></sub> separated by a&nbsp;space. These numbers form the given
sequence. The sequence can always be described by a&nbsp;polynomial <var>P</var>(<var>n</var>) 
such that for every <var>i</var>, 

<var>X</var><sub><var>i</var></sub> = <var>P</var>(<var>i</var>). Among these polynomials, we can find the
polynomial <var>P</var><sub><var>min</var></sub> with the lowest possible degree. This polynomial should be
used for completing the sequence.

</p><p>
</p><h3>Output</h3>

<p>

For every test case, your program must print a&nbsp;single line containing <var>C</var> 
integer numbers, separated by a&nbsp;space. These numbers are the values
completing the sequence according to the polynomial of the lowest possible
degree. In other words, you are to print values

<var>P</var><sub><var>min</var></sub>(<var>S</var>+1), <var>P</var><sub><var>min</var></sub>(<var>S</var>+2), .... <var>P</var><sub><var>min</var></sub>(<var>S</var>+<var>C</var>).


</p><p>
It is guaranteed that the results 
<var>P</var><sub><var>min</var></sub>(<var>S</var>+<var>i</var>) will be non-negative and
will fit into the standard <em>integer</em> type.

</p><h3>Example</h3>

<p>Sample Input:</p><pre><tt>4
6 3
1 2 3 4 5 6
8 2
1 2 4 7 11 16 22 29
10 2
1 1 1 1 1 1 1 1 1 2
1 10
3
</tt>
</pre>

<p>Sample Output:</p><pre><tt>7 8 9
37 46
11 56
3 3 3 3 3 3 3 3 3 3</tt>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>