<p>King Johnny of Byteland has in his short period of sovereignty established quite a few national holidays (close on thirty, in fact) in honour of... more or less anything he could think of. Each of these holidays occurs every a fixed number of days (possibly different for every holiday), and is accompanied by feasts, cabaret shows, and general merrymaking. Sometimes more than one holiday occurs on a single day, and once in a while all holidays take place on the same day. If this happens, the celebrations are combined and even more festive. After one such party, king Johnny started behaving strangely and had to be temporarily isolated from society.
</p><p>
For the period of king Johnny's absence (about 48 hours) you have been appointed Regent of Byteland. As a true patriot, you know that holidays are not good for the people, and would like to remove some before king Johnny returns (he won't mind, he never remembers anything after a party anyway). The people however, very sadly, don't know what is good for them, and will revolt if you remove more than k holidays. Try to choose the holidays you remove in such a way as to guarantee that the number of days which elapse between two consecutive holiday parties is as long as possible.
</p><p>
<b>Solve the problem in at most 4kB of source code.</b>

</p><h3>Input</h3>
<p>The first line of input contains a single integer t&lt;=200 - the number of test cases. t test case descriptions follow.
</p><p>
For each test case, the first line contains two space separated integers n k (1&lt;=k &lt; n&lt;=30), denoting the total number of holidays and the number of holidays to be removed. The next line contains n space separated integers, the i-th being t<sub>i</sub> (1&lt;=t<sub>i</sub>&lt;=10<sup>18</sup>) - the number of days every which the i-th holiday occurs.
</p><h3>Output</h3>
<p>For each test case, output one line containing an increasing sequence of exactly k integers - the numbers of the holidays to be removed (holidays are numbered in the input order from 1 to n).

</p><h3>Example</h3>

<pre><b>Input:</b>
1
5 2
6 13 10 15 7

<b>Output:</b>
2 5
</pre>
<p>
(The shortest period between two successive holiday parties is 2 days.)

</p>