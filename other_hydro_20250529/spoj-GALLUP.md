<p>Often, we see results of gallups, like this:
Prefer red: 3.5%
Prefer green: 4.5%
Prefer yellow: 22.0%
Prefer blue: 70.0%
and you begin to wonder: how many people did they really ask? If the numbers are simple, like 20%, 40%, and 40%, you know that they asked 5 people (or 10, or 15, or more, but we are interested in the minimum number of people).
Your task is to write a program that reads sets of percentages and calculates the smallest number of people that could produce the given percentages. We know that this number is always less than 10 000.

</p><h3>Input</h3>
<p>The input is a set of percentages. Each set is on a line of its own. Every line starts with an integer n (0 &lt;= n &lt;= 20) giving the number of percentages in the set. If n &gt; 0, the percentages follow as n numbers; these numbers may have 0�C5 decimals, and all percentages in a set have the same number of decimals. (If there are no decimals, there is no decimal point.) The percentages always add up to about 100% as there may be small rounding
errors. Numbers are rounded when digits are removed; they are rounded upwards if the first removed digit is 5 or more. Thus, 4.472 is rounded to 4.47, 4.5, or 4, depending on how many digits you want.

</p><h3>Output</h3>
<p>For each set of data, print a line starting with ��Case i :��, where ��i�� is the data set��s number. Then follows a space and an integer giving the computed number of people. If no legal answer in the range 1�C9999 exists,
print ��error�� instead of the number.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 20 40 40
3 33.3 33.3 33.3
2 33 67
1 100.0000
4 3.75 4.25 22.00 70.00
2 49 51
2 50 51
2 49 50
0

<b>Output:</b>
Case 1: 5
Case 2: 3
Case 3: 3
Case 4: 1
Case 5: 400
Case 6: 35
Case 7: 200
Case 8: error
</pre>