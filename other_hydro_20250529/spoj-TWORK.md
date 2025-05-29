<p>In the late Middle Ages the University of Byteland was no different than any other university of the day. One of those gloomy places where philosophers brooded over the essence of life, theologians did likewise and quaralled with philosophers, while alchemists developed new caustic types of green shampoo in their futile search for gold. The thing that worried the Chancellor most was that none of the staff seemed to be in the least capable of making money in any form. When he complained about this to the Director of Human Resources, the Director came up with a brilliantly simple theory. He claimed that this lack of productivity was the direct consequence of the isolated model of work, and that wonders could be achieved by promoting teamwork. </p><p>
The Director intends to assign every scientist to some 3-person workgroup. The members of the workgroup should then select which of them is to act as the group leader. And this of course is the root of the problem. Every scientist will tolerate either himself or one of his acquaintances as the leader of his group, but will never allow anyone else to have this privilege. So when creating workgroups it is necessary to bear in mind that every group should have at least one suitable candidate for the role of group leader, accepted by all its members.
</p><p>
Although everyone at the University knows <i>of</i> everyone else indirectly (as acquaintances of acquaintances of acquaintances of...), the number of direct acquaintances that every scientist has is relatively small - either equal to 2, or to 3. Even so, it ought to be possible to assign the vast majority of scientists to workgroups. Quite naturally, the dubious pleasure of performing this task has been left to you, the Acting University Algorithmist.

</p><h3>Input</h3>
<p>Input starts with a single integer t, the number of test cases (t&lt;=100). t test cases follow.</p><p>

Each test case begins with a line containing two integers n m (4&lt;=n&lt;=m&lt;=20000, n is the number of scientists and is divisible by 4). Exactly m lines follow containing a pair of integers a<sub>i</sub> b<sub>i</sub> each which denote that scientists a<sub>i</sub> and b<sub>i</sub> are acquaintances (1&lt;=a<sub>i</sub>, b<sub>i</sub>&lt;=n, each scientist has either 2 or 3 acquaintances). Acquaintanceship is mutual.

</p><h3>Output</h3>
<p>For each test case, output a line containing a single integer k - the number of workgroups you have formed. In each of the next k lines output exactly 3 integers, representing the numbers of scientists belonging to respective workgroups.
</p><p>Your solution will be regarded as incorrect if for some test case more than <i>25%</i> of all scientists are left without a valid assignment to a workgroup.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
8 10
1 2
1 3
2 5
4 6
3 7
2 3
5 6
6 7
7 8
8 4

<b>Output:</b>
2
1 3 7
4 5 6
</pre>