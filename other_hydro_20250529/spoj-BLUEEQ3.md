<h3>Background</h3>
<p>This morning Blue Mary wrote some equations on a piece of paper and left it on her desk.After solving some problems in SPOJ,she found that her classmate H.L. replaced all characters on the paper with some other ones.H.L. told her he replaced the same characters with the same ones,and different characters with different ones because of his goodness.Now Mary needs your help to get the original equations back.(See problem BLUEEQ)</p>
<h3>Input</h3>
<p>Ten test cases(given one after another,you have to process all!)For each test case, the first line is a single integer n(n&lt;=21).Next 3 lines contains 3 strings, each of them has a length of n and contains only first n capital latin characters.The sum of the numbers the first two strings indicates equals to the number the third string incicates.The numbers can have leading zeros and each of their bases is n.</p>
<h3>Output</h3>
<p>For each test case you should output one line contains n numbers separated by spaces, which is a permutation of integer numbers 0 to n-1.Number x is on the k-th position iff x is replaced by the kth capital latin character.There is one and only one solution for each test case.</p>
<h3>Example</h3>
<pre><b>Input:</b>
5
ABCED
BDACE
EBBAA
[and 9 test cases more]
<b>Output:</b>
1 0 3 4 2
[and 9 test cases more]
</pre>