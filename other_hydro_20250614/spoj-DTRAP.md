<pre><br><span style="white-space: normal;"><p>Dexter studies in Huber Elementary School, so does his arch rival Mandark. The school planned a fun trip to a carnival for N students. Everyone��s happy. Mandark has devised a plan to ruin the trip. He knows that there exist many groups within the students. Students of one group are friends with each other but not with any student of other groups. His plan is to instigate a fight among them.</p>
<p>At the carnival, all students line up for time on a trampoline. Dexter learns about Mandark��s plan and knows that If two students that are not friends get on the trampoline at the same time, a fight will start. Suddenly his ��lab alert�� buzzes. Deedee is trying to break into the lab again! Dexter has to get back home to defend his lab as soon as possible, but he can��t let Mandark ruin the trip.</p>
<p>The trampoline can handle a total weight of W kgs. The students are getting impatient to get on the trampoline. To save time and to avoid a fight, Dexter decides that he will select the first batch of&nbsp; students to go on the trampoline in such a way that their total weight exactly equals W and that no two students are not friends. Your job is to tell him&nbsp; the number of ways he can do&nbsp; this. Dexter has the knowledge of only M pairs of friends.&nbsp;</p>
<p><strong>INPUT:</strong></p>
<p>The first line contains T, the number test cases. T test cases follow. The first line of each test case contains three integers N, W and M. The next line contains N integers, The ith integer is the weight of the ith student (1&lt;=i&lt;=N). The next M lines contain two integers, q and w; this tells that student q and student w are friends.</p>
<p><strong>OUTPUT:</strong></p>
<p>For each test case, output a line containing a single integer, the number of ways Dexter can choose the first batch of students to get on the trampoline.</p>
<p><strong>CONSTRAINTS:</strong></p>
<p>1&lt;=T&lt;=10</p>
<p>1&lt;=N&lt;=22</p>
<p>1&lt;=q,w&lt;=N</p>
<p>0&lt;=M&lt;=(N*(N+1))/2</p>
<p>1&lt;=W&lt;=1500</p>
<p>1&lt;=Weight of each student&lt;=60</p>
<p>Assume that the max number of students on the trampoline has no limit. Only the max weight on the trampoline&nbsp; has the limit W.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE TEST CASES:</strong></p><p><strong>INPUT:</strong></p>
<p>2</p>
<p>10&nbsp; 90 5</p>
<p>20 30 10 20 30 50 40 20 40 50</p>
<p>1 2</p>
<p>2 3</p>
<p>3 4</p>
<p>4 5</p>
<p>9 10</p>
<p>5 57 3</p>
<p>20 10 96 20 1</p>
<p>1 2</p>
<p>2 3</p>
<p>1 3</p>
<p><strong>OUTPUT:</strong></p>
<p>3</p>
<p>0</p>
<p><strong>EXPLANATION:</strong></p>
<p>For first test case, the following three ways are possible. Using student number,</p>
<p>(1,2,3,5)</p>
<p>(2,3,4,5)</p>
<p>(9,10)</p>
<p>For the second test case, no way is possible for total weight of selected students to be exactly W.</p></span></pre>