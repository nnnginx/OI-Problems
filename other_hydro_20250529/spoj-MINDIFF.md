<p>You will be given three sorted arrays. Let¡¯s denote the three arrays as A, B and C.</p>
<p>Your task is fairly very simple. You just have to find one element from each of the three arrays so that <strong>(|A<sub>i</sub>-B<sub>j</sub>| + |B<sub>j</sub>-C<sub>k</sub>| + |C<sub>k</sub>-A<sub>i</sub>|)</strong> is the smallest.  Here A<sub>i</sub> is an element from array A. B<sub>j</sub> is an element form array B. C<sub>k</sub> is an element form array C.</p>
<h3>Input</h3>
<p>The first line of the input will be an integer T denote the number of test cases.</p>
<p>For each of the test cases there will three integers <strong>Na Nb Nc</strong> in the first line. Na will denote the size of array A, Nb will denote the size of array B, Nc will denote the size of array C.</p>
<p>In the second line of each test case there will be Na number of integers denoting the elements of array A.</p>
<p>In the third line of each test case there will be Nb number of integers denoting the elements of array B.</p>
<p>In the fourth line of each test case there will be Nc number of integers denoting the elements of array C.</p>
<h3>Output</h3>
<p>For each test case print the desired result.</p>
<h3>Constraints</h3>
<p>1 &lt;= t &lt;= 100<br> 1 &lt;= Na, Nb, Nc &lt;= 1000<br> Each elements of the arrays will be a non-negative number less than 10^9.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 2 3
2 4 6
5 7
1 3 5
3 5 4
1 3 5
7 8 9 10 11
2 14 20 36
</pre>
<pre><strong>Output:</strong>
2
10
</pre>