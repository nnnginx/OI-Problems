<p><em>Original problem statement (in Polish) can be found <a href="https://pizza.natodia.net/static/tasks/2015/eliminations/palisada.pdf">here</a>.</em></p>
<p>The year is 50 B.C. Gaul is entirely occupied by the Romans. Well, not entirely! One small village of indomitable Gauls still holds out against the invaders. And life is not easy for the Roman legionaries who garrison the fortified camps of Totorum, Aquarium, Laudanum and Compendium...</p>
<p>The year is 49 B.C. Gaul is entirely occupied by the Romans. Well, no one could seriously expect one small village to resist the mighty army of the great Roman Empire. Fortunately, thanks to Julius Caesar's infinite generosity (<em>Ave Caesar!</em>), the settlement wasn't razed to the ground. There was no other choice for the villagers than to conform to the new authorities.</p>
<p>But some of the rules of Roman law can be downright ridiculous. As it turns out, even heights of individual stakes in the stockade encircling the village are strictly regulated. Here is an excerpt from the law, laid down by Roman clerks, and approved by the great ruler, Gaius Julius Caesar (<em>Ave Caesar!</em>):</p>
<ul>
<li>Every stockade encircling every village in the whole Roman Empire (governed justly by the great Julius Caesar) should have even number of wooden logs.</li>
<li>Every log in every stockade should have some minimum height, specified in "Weights and Measures Act", article 15, passage 9. Moreover, the logs can be at most 1000 quarters of a sicilicus<sup>1</sup> higher than this minimum height.</li>
<li>For every log, the adjacent logs have to be both higher or both lower. It symbolizes the harmony in the whole Roman Empire, governed justly by the great Julius Caesar (<em>Ave Caesar!</em>).</li>
</ul>
<p><sup>1</sup><em>sicilicus</em> - Roman unit of length, equal to 1/48 of Roman foot.</p>
<p>As one might expect, stockade around the village of indomitable Gauls did not meet the requirements - specifically, it violated the last rule (it did satisfy the first two, though). Now, the villagers have to lower or raise some of the logs, but this is a lot of work. Determine the minimum number of logs that have to be lowered or raised, so that the final stockade will satisfy the rule of harmony.</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting the number of testcases. Then, testcases follow.</p>
<p>Each testcase consist of a single line. It begins with an integer <strong>n</strong>, indicating the number of logs in the stockade. (2 &lt;= <strong>n</strong> &lt;= 10<sup>6</sup>, 2 | <strong>n</strong>), followed by <strong>n</strong> integers <strong>x<sub>i</sub></strong>, indicating the difference between the height of the i-th log and the minimal possible height, expressed in quarters of a sicilicus (0 &lt;= <strong>x<sub>i</sub></strong> &lt;= 1000). i-th log is adjacent to (i+1)-th log, moreover, first log is adjacent to the last log (stockade encircles the village).</p>
<h3>Output</h3>
<p>For every testcase you should output one integer - minimum number of logs that have to be lowered or raised, so that the stockade satisfies the requirements of Roman law.</p>
<h3>Example</h3>
<p>Input:</p>
<pre>3
6 1 2 3 4 5 6
6 1 2 1 2 1 2
6 2 2 2 2 2 2</pre>
<p>Output:</p>
<pre>2
0
3</pre>
<h3>Explanation</h3>
<p>In the first case it is enough to lower the third and the fifth log to height 1. In the second case, the stockade already satisfies all the rules. (<em>Ave Caesar!</em>)</p>