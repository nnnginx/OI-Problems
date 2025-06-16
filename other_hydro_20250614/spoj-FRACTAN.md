To play the "fraction game" corresponding to a given list <code>f<sub>1</sub>, f<sub>2</sub>, ..., f<sub>k</sub></code> of fractions and starting integer <code>N</code>, you repeatedly multiply the integer you have at any stage (initially <code>N</code>) by the earliest <code>f<sub>i</sub></code> in the list for which the answer is integral.
Whenever there is no such <code>f<sub>i</sub></code>, the game stops.


<p></p><p>

Formally, we define a sequence by <code>S<sub>0</sub>=N</code>, and <code>S<sub>j+1</sub>=f<sub>i</sub>S<sub>j</sub></code>, if for <code>1&lt;=i&lt;=k</code>, the number <code>f<sub>i</sub>S<sub>j</sub></code> is an integer but the numbers <code>f<sub>1</sub>S<sub>j</sub>, ..., f<sub>i-1</sub>S<sub>j</sub></code> are not.


</p><p>

For example, if we have the list of eight fractions <code>f<sub>1</sub>=170/39</code>, <code>f<sub>2</sub>=19/13</code>, <code>f<sub>3</sub>=13/17</code>, <code>f<sub>4</sub>=69/95</code>, <code>f<sub>5</sub>=19/23</code>, <code>f<sub>6</sub>=1/19</code>, <code>f<sub>7</sub>=13/7</code>, <code>f<sub>8</sub>=1/3</code>, and start with <code>N=21</code>, we produce the (finite) sequence <code>(21,39,170,130,190,138,114,6,2)</code>.
In general, the sequence may be infinite.


</p><p>

Given a fraction list and a starting integer calculate a part of the defined sequence.
Actually, we are interested only in the powers of <code>2</code> that appear in the sequence.

</p><h3>Input Specification</h3><p>

The input contains several test cases.
Every test case starts with three integers <code>m, N, k</code>.
You may assume that <code>1&lt;=m&lt;=40</code>, <code>1&lt;=N&lt;=1000</code>, and <code>1&lt;=k&lt;=100</code>.
Then follow <code>k</code> fractions <code>f<sub>1</sub>, ..., f<sub>k</sub></code>.
For each fraction, first its numerator is given, followed by its denominator.
You may assume that both are positive integers less than <code>1000</code> and their greatest common divisor is <code>1</code>.
The last test case is followed by a zero.


</p><h3>Output Specification</h3><p>

For each test case output on a line <code>m</code> numbers <code>e<sub>1</sub>, ..., e<sub>m</sub></code>, separated by one space character, such that <code>2<sup>e<sub>1</sub></sup>, ..., 2<sup>e<sub>k</sub></sup></code> are the first <code>m</code> numbers in the defined sequence that are powers of <code>2</code>.
You may assume that there are at least <code>m</code> powers of <code>2</code> among the first 7654321 elements of the sequence.


</p><h3>Sample Input</h3><p>

</p><pre>1 21 8 170 39 19 13 13 17 69 95 19 23 1 19 13 7 1 3
20 2 14 17 91 78 85 19 51 23 38 29 33 77 29 95 23 77 19 1 17 11 13 13 11 15 2 1 7 55 1
0
</pre>

<h3>Sample Output</h3><p>

</p><pre>1
1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67
</pre>