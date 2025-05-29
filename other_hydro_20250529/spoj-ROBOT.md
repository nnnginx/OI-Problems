<p>Blue Mary, the well-known astronaut, had sent Robot No.1 to Mars finally.Robot No.1 was so smart that he could make one robot per second.</p>
<p>Assume the time Robot No.1 arrived was second 1. At second i, Robot No.1 made a new Robot: Robot No.i. (i&gt;=2)</p>
<p>The new robots started work as soon as he was produced successfully. Robot No.M only had a rest at second t, where t is a multiple of M. 
For example, Robot No.3 worked at second 4,5,7,8,... and had a rest at second 6,9,...</p>
<p>When a robot was having a rest, he could send his own informations to the newly produced robot. For example, when Robot No.6 was produced successfully,
Robot No.2 and Robot No.3 are having a rest, so Robot No.6 would get informations from Robot No.2 and No.3. We call Robot No.2 and No.3 are teachers of
Robot No.6. </p>
<p>We call two Robots are independent if each of them wasn't a teacher of the other one and they had no common teachers. <b>Please note that Robot No.1
was independent to any other robots and wasn't a teacher of any other robots, </b>since only Robot No.1 could make robots.</p>
<p>The good number of Robot No.M is the number of robots who was produced earlier than No.M and independent to No.M. Here are some examples: </p>
<p>The good number of Robot No.1 is 0.</p>
<p>The good number of Robot No.2 is 1. No.1 was that robot.</p>
<p>The good number of Robot No.6 is 2. No.1 and No.5 were those robots. No.2 and No.3 were his teachers. No.4 and him had a common teacher: No.2. </p>
<p>The Robots had 3 kinds of occupations. To Robot No.M:</p>
<div align="justify">
       <ul>
               <li>
               If M can be written as the multiple of an even number of distinct odd primes, he was a businessman.
               </li><li>
               If M can be written as the multiple of an odd number(1 included) of distinct odd primes, he was a hacker.
               </li><li>
               All other robots were doctors.</li>
       </ul>
</div>
<p>Now Blue Mary was interesting to Robot No.M. She wants to know the sum of good numbers of all businessmen, hackers and doctors among Robot No.M and his teachers.
She comes up with the answer quickly, and so can you.</p>
<p>Blue Mary is so kind that she gives you the prime divisors of M and you can only tell her the answers modudo 10000.</p>
<h3>Input</h3>
<p>The very first line contains a single integer T,the number of test cases.T blocks follow. </p>
<p>For each block, the first line contains a single integer K.K lines follow, each contains two integers p<sub>i</sub> and a<sub>i</sub> separated by a single space.</p>
<p>M = p<sub>1</sub><sup>a<sub>1</sub></sup> * p<sub>2</sub><sup>a<sub>2</sub></sup> * p<sub>3</sub><sup>a<sub>3</sub></sup> * ... * p<sub>K</sub><sup>a<sub>K</sub></sup>. </p>
<p>You can assume that:</p>
<div align="justify">
       <ul>
               <li>
               All p<sub>i</sub> are distinct primes and are less than 10,000.
               </li><li>
               p<sub>1</sub> &lt; p<sub>2</sub> &lt; p<sub>3</sub> &lt; ... <p<sub>n.
               </p<sub></li><li>
               All a<sub>i</sub> are positive and no more than 1,000,000.
               </li><li>
               1 &lt;= k &lt;= 1000.</li>
       </ul>
</div>
<h3>Output</h3>
<p>For each test case, output 3 lines. </p>
<p>The first line contains a single integer denotes to the sum of good numbers of all businessmen among Robot No.M and his teachers modudo 10000. </p>
<p>The second line contains a single integer denotes to the sum of good numbers of all hackers among Robot No.M and his teachers modudo 10000.</p>
<p>The third line contains a single integer denotes to the sum of good numbers of all doctors among Robot No.M and his teachers modudo 10000.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
3
2 1
3 2
5 1

<b>Output:</b>
8
6
75
</pre>
<h3>Hints</h3>
<p>In the sample input, M=2<sup>1</sup>*3<sup>2</sup>*5<sup>1</sup>=90. Robot No.90 has 10 teachers.Among Robot No.90 and his teachers, Robot No.15 is a businessman; No.3 and No.5
are hackers; all others are doctors, their numbers are 2,6,9,10,18,30,45,90.</p>