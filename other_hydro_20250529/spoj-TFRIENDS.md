<p>You are given a string array representing Known people. Known[i][j]='Y' if i knows j.<br><br></p>
<p><strong>Friends:</strong> A is a friend of B if B knows A or B has a friend who knows A.<br><br></p>
<p><strong>True friends:</strong> A and B are true friends if A is a friend of B and B is a friend of A.<br><br></p>
<p><strong>Group:</strong> Everyone in a Group must be true friends to each other.<br><br></p>
<p>Your task is to find the number of Groups from the given list of Known people. It can be proved that there is exactly only one possible way for forming the groups.<br><br></p>
<p><strong>Input:</strong> The first line consists of an integer t, the number of test cases. For each test case, you are given an array of strings representing Known people. Known is of size NxN where N is the total number of people. <br><br></p>
<p><strong>Output:</strong> For each test case, print the number of Groups. <br><br></p>
<p><strong>Input Constraints:</strong></p>
<p>1&lt;=t&lt;=1000</p>
<p>1&lt;=N&lt;=100</p>
<p>Known[i][j] is either 'Y' or 'N'</p>
<p>Known[i][i]='N' (No one is known to themselves) <br><br></p>
<p><strong>Sample Input:</strong></p>
<pre>3
3
NYN
NNY
YNN
7
NNYNNNN
NNNYYYN
NNNNNNN
YNNNNNN
NNNYNNN
NNNNNNN
NNNNNYN
7
NNNNYYN
NNNNNNN
NNNNNYN
NYNNNYY
NNNYNNN
NNYNNNY
NNNNYNN</pre>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<pre>1
7
3</pre>
<p>&nbsp;</p>
<p><strong>Explanation:</strong></p>
<p><strong>Case 1:</strong> All the friends are true friends to each other</p>
<p><strong>Case 2:</strong> No two true friends exist.</p>
<p><strong>Case 3:</strong> There are 3 groups of true friends. {0}, {1}, {2,3,4,5,6}</p>