<p>You are to write a program to perform some operations on a given sequence.These operations are listed below:</p>
<pre>---------------------------------------------------------------------------------------------
| Name        | Input format   |              function                                      |
---------------------------------------------------------------------------------------------
| Modify      | MAKE-SAME i t c| Modify all the t numbers from the ith number(included) to  |
|             |                | number c.                                                  |
---------------------------------------------------------------------------------------------
| Insert      | INSERT i t s   | Insert t numbers after the ith number.s is a sequence of t |
|             |                | numbers which should be inserted one-to-one.If i=0,you     |
|             |                | should insert s in the first of the sequence.              |
---------------------------------------------------------------------------------------------
| Delete      | DELETE i t     | Delete t numbers after the ith number(included).           |
---------------------------------------------------------------------------------------------
| Reverse     | REVERSE i t    | Reverse t numbers after the ith number(included).          |
---------------------------------------------------------------------------------------------
| Get sum     | GET-SUM i t    | Output the sum of t numbers after the ith number(included).|
---------------------------------------------------------------------------------------------
| Get maximum | MAX-SUM        | Output the maximum partial sum in the sequence now.        |
| partial sum |                |                                                            |
---------------------------------------------------------------------------------------------
</pre>
<p>See the example.</p>
<h3>Input</h3>
<p>The very first line contains a single integer T(T&lt;=4), the number of test cases.T blocks follow.</p>
<p>For each test case: </p>
<p>The first line contains two integers n and m(m&lt;=20000), the number of numbers in the sequence in the beginning and the 

number of operations.</p>
<p>The second line contains n integers seperated by spaces, the sequence in the beginning.</p>
<p>Next m lines, each contains an operation listed above.</p>
<p>You can assume that for each test case:</p>
<div align="justify">
    <ul>
        <li>
        No invalid operation is in the input.
        </li><li>
        Number of numbers in the sequence is no more than 500000 and not less than 1 at any time.
        </li><li> 
        All the numbers in the sequence is in range[-1000,1000] at any time.
        </li><li>
        The total number of numbers inserted will be not more than 4,000,000.The input is no more than 20MB.
        </li>
    </ul>
</div>
<h3>Output</h3>
<p>For each Get sum and Get maximum partial sum operation,you should write the answer to the output,one per line.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
9 8
2 -6 3 5 1 -5 -3 6 3
GET-SUM 5 4
MAX-SUM
INSERT 8 3 -5 7 2
DELETE 12 1
MAKE-SAME 3 3 2
REVERSE 3 6
GET-SUM 5 4
MAX-SUM

<b>Output:</b>
-1
10
1
10

<b>Hints:</b>
<p>After the 3rd op., the sequence is </p>
2 -6 3 5 1 -5 -3 6 -5 7 2 3

<p>After the 4th op., the sequence is </p>
2 -6 3 5 1 -5 -3 6 -5 7 2

<p>After the 5th op., the sequence is </p>
2 -6 2 2 2 -5 -3 6 -5 7 2

<p>After the 6th op., the sequence is </p>
2 -6 6 -3 -5 2 2 2 -5 7 2

</pre>
<b>Warning: enormous Input/Output data, be careful with certain languages</b>