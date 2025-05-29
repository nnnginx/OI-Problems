<p align="left">Archaeologists have made a discovery on the Temple of Topology. The temple was once used as a place for ritual ceremony thousands of years ago. Among the relics that were unearthed, a scroll of parchment raised the interest of scientists. The parchment contained many numbers written in ancient symbols.</p>
<p align="left">By decrypting the words carved on a stone, scientists know that these numbers form an interesting set of integers satisfying the following two properties:</p>
<p align="left">1. Bitwise AND any number of integers from the set result in an integer in that set again.</p>
<p align="left">2. Bitwise OR any number of integers from the set result in an integer in that set again.</p>
<p align="left">As the parchment is extremely old, some part of it were broken and the numbers were lost. Now you job is to complete the original set from the remaining integers such that the size of the set is as small as possible.</p>
<h3>Input</h3>
<p align="left">The input contains several test cases. The total number of test cases is less than 1100. Each test case begins with a line containing an integer <strong>n</strong> (<strong>n</strong> &gt; 1). The following line contains <strong>n</strong> integers <strong>a<sub>i</sub></strong> (0 &lt;= <strong>a<sub>i</sub></strong> &lt; 2<sup>16</sup>), the remaining integers on the parchment. The integers are distinct.</p>
<h3>Output</h3>
<p align="left">For each test case, output one line containing a single integer, the minimal number of additional integers to make the set complete. If these numbers are already a complete set, print 0.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
5
0 1 3 5 7
2
2 4
3
3 7 11
3
1 2 4

<strong>Output:</strong>
Case #1: 0
Case #2: 2
Case #3: 1
Case #4: 5
</pre>