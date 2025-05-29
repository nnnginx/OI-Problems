<div>
<p>It's unbelievable, but an exam period has started at the OhWord  University. It's even more unbelievable, that Valera got all the tests  before the exam period for excellent work during the term. As now he's  free, he wants to earn money by solving problems for his groupmates.  He's made a <span><em>list</em></span> of subjects that he can help with. Having spoken with <span><em>n</em></span> of his groupmates, Valera found out the following information about  them: what subject each of them passes, time of the exam and sum of  money that each person is ready to pay for Valera's help.</p>
<p>Having  this data, Valera's decided to draw up a timetable, according to which  he will solve problems for his groupmates. For sure, Valera can't solve  problems round the clock, that's why he's found for himself an optimum  order of day and plans to stick to it during the whole exam period.  Valera assigned time segments for sleep, breakfast, lunch and dinner.  The rest of the time he can work.</p>
<p>Obviously, Valera can help a student with some subject, only if this subject is on the <span><em>list</em></span>.  It so happenes, that all the students, to whom Valera spoke, have different, but one-type problems. Valera can solve any  problem of subject <span><em>list</em><sub><em>i</em></sub></span> in <span><em>t</em><sub><em>i</em></sub></span> minutes.</p>
<p>Moreover,  if Valera starts working at some problem, he can break off only for  sleep or meals, but he can't start a new problem, not having finished  the current one. Having solved the problem, Valera can send it instantly  to the corresponding student via the Internet.</p>
<p>If this student's  exam hasn't started yet, he can make a crib, use it to pass the exam  successfully, and pay Valera the promised sum. Since Valera has little  time, he asks you to write a program that finds the order of solving  problems, which can bring Valera maximum profit.</p>
</div>
<div>
<h3>Input</h3>
<p>The first line contains integers <span><em>m</em>, <em>n</em>, <em>k</em></span> (<span>1 ≤ <em>m</em>, <em>n</em> ≤ 100</span>, <span>1 ≤ <em>k</em> ≤ 30</span>) — amount of subjects on the <span><em>list</em></span>, amount of Valera's potential employers and the duration of the exam period in days.</p>
<p>The following <span><em>m</em></span> lines contain the names of subjects <span><em>list</em><sub><em>i</em></sub></span> (<span><em>list</em><sub><em>i</em></sub></span> is a non-empty string of at most 32 characters, consisting of lower  case Latin letters). It's guaranteed that no two subjects are the same.</p>
<p>The <span>(<em>m</em> + 2)</span>-th line contains <span><em>m</em></span> integers <span><em>t</em><sub><em>i</em></sub></span> (<span>1 ≤ <em>t</em><sub><em>i</em></sub> ≤ 1000</span>) — time in minutes that Valera spends to solve problems of the <span><em>i</em></span>-th subject. Then follow four lines, containing time segments for sleep, breakfast, lunch and dinner correspondingly.</p>
<p>Each line is in format <span>H1:M1-H2:M2</span>, where <span>00 ≤ </span> <span>H1</span>, <span>H2</span> <span> ≤ 23</span>, <span>00 ≤ </span> <span>M1</span>, <span>M2</span> <span> ≤ 59</span>. Time <span>H1:M1</span> stands for the first minute of some Valera's action, and time <span>H2:M2</span> stands for the last minute of this action. No two time segments cross.  It's guaranteed that Valera goes to bed not before midnight, gets up earlier  than he has breakfast, finishes his breakfast before lunch, finishes  his lunch before dinner, and finishes his dinner before midnight. All  these actions last less than a day, but not less than one minute. Time  of the beginning and time of the ending of each action are within one  and the same day. But it's possible that Valera has no time for solving  problems.</p>
<p>Then follow <span><em>n</em></span> lines, each containing the description of students. For each student the following is known: his exam subject <span><em>s</em><sub><em>i</em></sub></span> (<span><em>s</em><sub><em>i</em></sub></span> is a non-empty string of at most 32 characters, consisting of lower case Latin letters), index of the exam day <span><em>d</em><sub><em>i</em></sub></span> (<span>1 ≤ <em>d</em><sub><em>i</em></sub> ≤ <em>k</em></span>), the exam time <span><em>time</em><sub><em>i</em></sub></span>, and sum of money <span><em>c</em><sub><em>i</em></sub></span> (<span>0 ≤ <em>c</em><sub><em>i</em></sub> ≤ 10<sup>6</sup></span>, <span><em>c</em><sub><em>i</em></sub></span> — integer) that he's ready to pay for Valera's help. Exam time <span><em>time</em><sub><em>i</em></sub></span> is in the format <span>HH:MM</span>, where <span>00 ≤ </span> <span>HH</span> <span> ≤ 23</span>, <span>00 ≤ </span> <span>MM</span> <span> ≤ 59</span>. Valera will get money, if he finishes to solve the problem strictly before the corresponding student's exam begins.</p>
</div>
<div>
<h3>Output</h3>
<p>In the first line output the maximum profit that Valera can get. The second line should contain number <span><em>p</em></span> — amount of problems that Valera is to solve. In the following <span><em>p</em></span> lines output the order of solving problems in chronological order in  the following format: index of a student, to whom Valera is to help;  index of the day, when Valera should start the problem; time, when  Valera should start the problem (the first minute of his work); index of  the day, when Valera should finish the problem; time, when Valera  should finish the problem (the last minute of his work). To understand  the output format better, study the sample tests.</p>
</div>
<h3>Sample tests</h3>
<div>
<div>Input</div>
<pre>3 3 4<br>calculus<br>algebra<br>history<br>58 23 15<br>00:00-08:15<br>08:20-08:35<br>09:30-10:25<br>19:00-19:45<br>calculus 1 09:36 100<br>english 4 21:15 5000<br>history 1 19:50 50<br></pre>
</div>
<div>
<div>Output</div>
<pre>150<br>2<br>1 1 08:16 1 09:29<br>3 1 10:26 1 10:40<br></pre>
</div>
<div>
<div>Input</div>
<pre>2 2 1<br>matan<br>codeforces<br>1 2<br>00:00-08:00<br>09:00-09:00<br>12:00-12:00<br>18:00-18:00<br>codeforces 1 08:04 2<br>matan 1 08:02 1<br></pre>
</div>
<div>
<div>Output</div>
<pre>3<br>2<br>2 1 08:01 1 08:01<br>1 1 08:02 1 08:03<br></pre>
</div>
<div>
<div>Input</div>
<pre>2 2 1<br>matan<br>codeforces<br>2 2<br>00:00-08:00<br>09:00-09:00<br>12:00-12:00<br>18:00-18:00<br>codeforces 1 08:04 2<br>matan 1 08:03 1<br></pre>
</div>
<div>Output</div>
<pre>2<br>1<br>1 1 08:01 1 08:02</pre>