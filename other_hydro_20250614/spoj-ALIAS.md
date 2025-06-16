<p>Alias is an assumed or additional name that constitutes a distinctive designation of a person. Consider a set of n  persons and assume that each person has k  distinct aliases. A person is identified using any one of its k  aliases. The nk  (= n¡Ák)  distinct aliases are identified using integers 1, 2,...nk . Integers 1, 2,..., n  represent the first aliases of all n  persons in an arbitrary order. In general, integers (j - 1)¡Án + 1,(j - 1)¡Án + 2,...,(j - 1)¡Án + n  represent the jth  alias of all n persons in an arbitrary order, for j = 1, 2,..., k . Persons in the set are totally ordered with respect to a quality characteristic Q  associated with each person. Let Q(r)  be the value of Q  for a person identified by one of its alias r .</p>
<p>
Given a sufficient number, say m , of inequalities of the type: Q(r) &gt; Q(s) , you are required to write a program to sort all persons in descending order and recognize all aliases of each person in the set.
</p>
<p>
As a simple illustration consider distinct total marks scored by three students in an examination. Each student is identified by any one of three distinct aliases in the Name: {first-name middle-name last-name}. Let integers 1, 2, 3 represent the first names, 4, 5, 6 represent the middle names and 7, 8, 9 represent the last names in an arbitrary order. Let Q(r) be the total marks of student r, r being an alias. Given the following inequalities: Q(6) &gt; Q(1), Q(9) &gt; Q(4), Q(5) &gt; Q(8), Q(2) &gt; Q(9), Q(7) &gt; Q(3), Q(9) &gt; Q(3) , one can conclude that the names of students appearing in descending order of total marks are {2 6 7}, {1 5 9} and {3 4 8}.
</p>
<h3>Input</h3>
<p>
The input may contain multiple test cases.
</p>
<p>For each test case the first input line gives the parameters n , k and m .
</p>
<p>
The second line contains m inequalities represented by 2¡Ám integers. An integer r occurring in an odd numbered position in the line and the integer s occurring in the next even numbered position, represent the inequality Q(r) &gt; Q(s) .
</p>
<p>
Assume that nk is less than 100 and each integer in the second input line is of two digits, including a non-significant 0 when required.
</p>
<p>
The input terminates with a line containing 0 as input.
</p>
<h3>Output</h3>
<p>
For each test case print n lines giving k aliases of each person in a line; a line contains aliases in increasing order. Arrange persons in descending order of the quality characteristic Q . As in input, each integer in output is of two digits, including a non-significant 0 when required.
</p>
<p>
A blank line appears after the last output line of a test case.
</p>
<h3>Example</h3>
<pre><b>Sample Input</b>
3 3 6
06 01 09 04 05 08 02 09 07 03 09 03
2 4 2
03 08 02 05
0

<b>Sample Output</b>
02 06 07
01 05 09
03 04 08

02 03 06 07
01 04 05 08
</pre>