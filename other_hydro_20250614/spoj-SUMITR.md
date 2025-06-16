<p>
Let us consider a triangle of numbers in which a number appears in the first line, two 
numbers appear in the second line etc. Develop a program which will compute the largest 
of the sums of numbers that appear on the paths starting from the top
towards the base, so that:
</p><ul>
<li> on each path the next number is located on the row below, more precisely 
either directly below or below and one place to the right;
</li>
<li>
the number of rows is strictly positive, but less than 100;
</li>
<li> all numbers are positive integers between O and 99.
</li>
</ul>
<p>
Take care about your fingers, do not use more than <b>256</b> bytes of code. 

</p><h3>Input</h3>
<p>
In the first line integer n - the number of test cases (equal to about 1000). 
Then n test cases follow. Each test case starts with the number of lines which is followed by their content.
</p><h3>Output</h3>
<p>
For each test case write the determined value in a separate line. 


</p><h3>Example</h3>

<pre><b>Input:</b>
2
3
1
2 1
1 2 3
4 
1 
1 2 
4 1 2
2 3 1 1 

<b>Output:</b>
5
9
</pre>

<b>Warning: large Input/Output data, be careful with certain languages</b>