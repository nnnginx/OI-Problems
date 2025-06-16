<p>Mr. B and Mr. M like to play with balls. They have many balls colored in blue and red. Firstly, Mr. B randomly picks up <strong>N</strong> balls out of them and put them into a bag. Mr. M knows that there are <strong>N</strong>+1 possible situation which the number of red balls are ranged from 0 to <strong>N</strong>, and we assume the possibilities of the <strong>N</strong>+1 situation are the same. But Mr. M does not know which situation occurs. Secondly, Mr. M picks up P balls out of the bag and examines them. There are <strong>Q</strong> red balls and <strong>P</strong>-<strong>Q</strong> blue balls. The question is, if he picks one more ball out of the bag, what is the possibility that this ball is red.</p>
<h3>Input</h3>
<p>Each test case contains only one line with three integers <strong>N</strong>, <strong>P</strong> and <strong>Q</strong> (2 &lt;= <strong>N</strong> &lt;= 100,000, 0 &lt;= <strong>Q</strong> &lt;= <strong>P</strong> &lt;= <strong>N</strong>-1).</p>
<h3>Output</h3>
<p>For each test case, display a single line containing the case number and the possibility of the next ball Mr. M picks out is red. The number should be round to four decimal places.</p>
<p><strong>The judge is "ignoring extra whitespaces".</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 0 0
4 2 1

<strong>Output:</strong>
Case 1: 0.5000
Case 2: 0.5000
</pre>
<p><strong>Explanation</strong></p>
<p>For example as the sample test one, there are three balls in the bag. The possibilities of the four possible situations are all 0.25. If there are no red balls in the bag, the possibility of the next ball are red is 0. If there is one red ball in the bag, the possibility is 1/3. If there are two red balls, the possibility is 2/3. Finally if all balls are red, the possibility is 1. So the answer is 0*(1/4)+(1/3)*(1/4)+(2/3)*(1/4)+1*(1/4)=0.5.</p>