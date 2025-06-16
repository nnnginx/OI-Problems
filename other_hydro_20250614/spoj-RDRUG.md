<p>Dr. Banner (a.k.a. The Hulk) is synthesizing a drug that will help him control his rage. There are a total of N atoms of various atomic masses. <br> Banner knows that to create a bond between two atoms the energy required  is equal to the sum of the atomic masses of the two atoms. <br> Currently some of the atoms are connected to one another forming compounds. <br> Banner wants to join all separate atoms and compounds into a single  compound by creating chemical bonds. Each atom can form at max one more  bond. Help Dr. Banner to find out the minimum energy required to  synthesize his drug.</p>
<h4>INPUT</h4>
<p>Input starts with an integer T, the number of test cases. Each test case  starts with a line containing integers N, M denoting the number of  atoms and the number of bonds already formed respectively. M lines contain 2 integers i and j denoting a chemical bond between the  ith and the jth atom. The next N lines contains one integer each where the integer on ith line  denotes the atomic mass of the ith atom.</p>
<h4>OUTPUT</h4>
<p>Print T lines, where the ith line is the answer to the ith test case. If it is not possible to link the atoms print -1;  <br> PS: If you mislead Dr. Banner, he might lose his temper and SMASH you to bits. <br><br></p>
<h4>CONSTRAINTS</h4>
<p>1 &lt;= T &lt;= 12 <br> 1 &lt;= N &lt;= 100000 <br> 1 &lt;= AtomicMass &lt;= 10000 <br> 1 &lt;= M &lt;= 10^6 (1000000) <br> 1 &lt;= i, j  &lt;= N</p>
<h4>Sample Input:</h4>
<pre>2
6 6
1 2
2 3
1 3
4 5
5 6
4 6
1
3
5
2
4
6
4 0
1
2
3   
4


</pre>
<h4>Sample Output:</h4>
<p>3 <br> -1</p>