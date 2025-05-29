<p>Mr. B is the chief engineer in the Kingdom of FDUCS. Recently, the King asks Mr. B to develop a new plan of the road network in the country, since the existing one is so old that traffic jam often occurs. Unfortunately, Mr. B is now preparing for the ICPC World Final Contest so that he is quite busy. He asks his friends, Mr. G and Mr. M to help him finish that work. When Mr. B gets the solution from his friends, he realizes some problems: Mr. B forgot to specify the budget plan to Mr. G and Mr. M, thus the new solution contains too many new roads which the government cannot afford. After a precise calculation, Mr. B finds that he has just to delete exactly two roads in term of the financial facts (Of course, Mr. B will not delete more than two roads because he wants people in his country to have a convenient traffic).</p>
<p>Can Mr. B delete two roads arbitrarily? The answer is negative. The King would like to take a travel on the new road system to review Mr. B's work. However, the King is so busy that he does not want to take travel with redundancy. That is, the King wants Mr. B to design a road system so that he can travel from the palace (in one city), pass each road exactly once, and then back to the palace. Moreover, during his travelling, the king must visit each city at least once too.</p>
<p>Mr. B feels hard to satisfy the Kings demand by deleting two roads from the original design. As an ICPC candidate with unlimited potential, can you help him?</p>
<h3>Input</h3>
<p>For each test case, the first line contains two integers, <strong>n</strong> and <strong>m</strong> (1 &lt;= <strong>n</strong>, <strong>m</strong> &lt;= 200,000), indicating the number of cities in the Kingdom and the roads in Mr. B's original plan. Following this are <strong>m</strong> lines, each contains a pair of integers <strong>a</strong> and <strong>b</strong>. Each of them denotes <strong>a</strong> bidirectional road between city <strong>a</strong> and city <strong>b</strong> (1 &lt;= <strong>a</strong>, <strong>b</strong> &lt;= n and <strong>a</strong> != <strong>b</strong>), the number of cities are counted from 1. No two roads connect the same pair of cities.</p>
<h3>Output</h3>
<p>For each test case, if Mr. B can satisfy the Kings requirement, then output <strong>YES</strong> in the first line, otherwise, output <strong>NO</strong>. If the answer is <strong>YES</strong>, output two integers <strong>X</strong> and <strong>Y</strong> (<strong>X</strong> &lt; <strong>Y</strong>) in the following line, specifying two roads that Mr. B should delete from the original design. <strong>X</strong> and <strong>Y</strong> are the indexes of roads in the input, counting from 1. If there are more than one possible answer, output the one that makes the pair of (<strong>X</strong>, <strong>Y</strong>) lexicographically smallest.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 6
1 2
1 3
1 4
2 3
2 4
3 4

<strong>Output:</strong>
Case 1: YES
1 6
</pre>