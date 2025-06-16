<p>Blue Mary is a cashier of a big company.The boss of this company is so annoying that he always increases or decreases wage of all workers.He increases all the workers' wage with a same number when he is happy or decreases all the worker's wage with a same number when he is depressed. </p>
<p>All the workers are angry with the boss, especially when he decreases their wage. A worker will leave the company and never go back when he finds his wage is lower than the least wage written on his contract. Blue Mary must delete the worker's files at that time. Another task she is to do is to build a file when a new worker joins this company.</p>
<p>The boss usually asks Blue Mary how much money the worker who gets the k-th most wage gets. Blue Mary is very tired with her work. Could you give her a hand?</p>
<h3>Input</h3>
<p>T</p>
<p>[the number of tests &lt;= 10]</p>
<p>M MIN</p>
<p>[M is the number of commands below, MIN is the least wage]</p>
<p>C K</p>
<p>[C is one of the 4 characters I,A,S,F. I denotes that Mary should build a new file, and the new worker's wage is K(0&lt;=K&lt;=100000) at start.If K is less than MIN, the worker will not join the company. A denotes that the boss increases all the workers' wage with K(0&lt;=K&lt;=1000). S denotes that the boss decreases all the workers' wage with K(0&lt;=K&lt;=1000). F denotes that the boss asks Blue Mary a question: how much money does the worker who gets the k-th most wage get(K&gt;0)?]</p>
<p>[M-1 other commands]</p>
<p>[other tests]</p>
<p>You may assume that:</p>
<div align="justify">
    <ul>
        <li>
        The number of worker in the company at start is 0.
        </li><li>
        The number of command I is no more than 100000.
        </li><li>
        The total numner of command A and S is no more than 100.
        </li><li>
        The number of command F is no more than 100000.</li>
    </ul>
</div>
<h3>Output</h3>
<p>For each test case:</p>
<p>For each F command you must output one line contains a single integer which is the answer or -1 if K is more than the number of workers in the company at that time.</p>
<p>In the last line you must output a single integer - the number of workers who leave the company(excluded the ones who don't join the company)</p>
<h3>Example</h3>
<pre><b><tt>Sample Input:</tt></b>
1
9 10
I 60
I 70
S 50
F 2
I 30
S 15
A 5
F 1
F 2

<b><tt>Sample Output:</tt></b>
10
20
-1
2
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>