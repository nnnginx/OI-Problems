<p>

The Bogus Corporation distributes salary to its employees in a weird
manner. The salary is distributed every <span style="font-weight: bold;">K</span> days,
&nbsp;and instead of same salary for each day, the salary for the i<sup>th</sup>
day is a<sub>i</sub>. An ambitious young manager, fresh
from <span style="font-style: italic;">Institute of
Mismanagement, </span>observes that people usually prefer to
take leave towards the end of this period of K days, when the workload
is higher. Instead of revising each of the a<sub>i</sub>'s,
the manager comes up with a quick fix solution - he redefines
the new salary on the i<sup>th</sup> day as b<sub>i</sub>=a<sub>i</sub>+2a<sub>i-1</sub>+2<sup>2</sup>a<sub>i-2</sub>+2<sup>3</sup>a<sub>i-3</sub>+........+2<sup>i-1</sup>a<sub>1</sub>
. Baba, one of the employees, is in a dire financial crisis, and must
accumulate at least<span style="font-style: italic;"> </span><span style="font-weight: bold;">N</span> rupees at the end
of the forthcoming period. Being a lazy worker that he is, he is
interested in finding out if attending particular days would guarantee
him <span style="font-style: italic;">exactly</span>
&nbsp;<span style="font-weight: bold;">N</span>
rupees at the end of the period. Can you help Baba?




</p><h3>Input</h3>
<p>

First line contains a single integer integer <span style="font-weight: bold;">T</span>, the number of
test cases ( 1&lt;=T&lt;=100). Each test case is described on
two lines. First line contains two integers, <span style="font-weight: bold;">N</span> and <span style="font-weight: bold;">K</span> (
1&lt;=N&lt;=2<sup>63</sup>-1,
1&lt;=K&lt;=50) , the second line contains a space separated
list of K integers, the <span style="font-weight: bold;">a</span><sub style="font-weight: bold;">i</sub><span style="font-weight: bold;">'s</span> ( 1&lt;=a<sub>i</sub>&lt;=1000).


</p><h3>Output</h3>
<p>

For each test case, output on a single line 1-based indices of the days
(separated by a single space) he should attend to ensure a salary of
exactly N rupees at the end of the period. The indices should be
printed in the sorted order. In case of multiple answers, output any
one of them. If there is no answer, print -1.


</p><h3>Example</h3>

<pre><b>Input:</b>
2
9 3
1 1 2
10 2
2 3
<b>Output:</b>
1 3
-1
</pre>