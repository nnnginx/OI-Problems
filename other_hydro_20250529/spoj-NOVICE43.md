<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">When I first learned backtracking I made a program to find all the permutations of the English alphabets in lexicographically increasing. Filled with elation I showed the program to Rohil. Rohil being someone who likes to do stuff off the league was not impressed and gave me the following variation of the problem help me to solve the problem:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You have to find the number of permutations of length N(1&lt;=N&lt;=12) such that at whenever an alphabet say($) appears in the permutation all the alphabets smaller than $ should have appeared before it at least once. An alphabet is smaller than another if it appears before the other in the English alphabet. ¡®a¡¯ being the smallest and ¡®z¡¯ being the largest. For example when N=2 then aa,ab are the only valid permutations and ba,bb is invalid since in ba all the alphabets smaller than b have not appeared at least once before it. See example for further clarification.</div>
<p>When I first learned backtracking I made a program to find all the permutations of the English alphabets in lexicographically increasing. Filled with elation I showed the program to Rohil. Rohil being someone who likes to do stuff off the league was not impressed and gave me the following variation of the problem help me to solve the problem:&nbsp;</p>
<p>You have to find the number of permutations of length N(1&lt;=N&lt;=11) such that at whenever an alphabet (say 'c' ) appears in the permutation all the alphabets smaller than 'c' should have appeared before it at least once. An alphabet is smaller than another if it appears before the other in the English alphabet. ¡®a¡¯ being the smallest and ¡®z¡¯ being the largest. For example when N=2 then aa,ab are the only valid permutations and ba,bb is invalid since in ba all the alphabets smaller than b have not appeared at least once before it. See example for further clarification.</p>
<h3>Input</h3>
<p>Line 1: T(no. of test cases)</p>
<p>Line 2: n1</p>
<p>Line 3: n2</p>
<p>¡­</p>
<p>¡­</p>
<h3>Output</h3>
<p>Line 1: no. of such permutations of length n1</p>
<p>¡­¡­</p>
<p>¡­..</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
3

<strong>Output:</strong>
2
5</pre>
<pre>Explanation for N=3, the possible permutations are:
abc
aba
abb
aab
aaa</pre>