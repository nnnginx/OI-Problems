<h2 align="center">help the Prayatna pr team</h2>
<p>Well, the annual technical symposium of Department of Computer Technology is around the corner. All that we need, to make it a grand success is Publicity among the peer groups ( ofCourse the sponsors too :P ). We decided to share the job between the student groups. As per the plan we decided to meet people in person and influence them to attend Prayatna. But to meet them we have to go to various student groups. To do so, we had to cut our classes. But being studious. students refused to cut more classes. Instead of meeting every one in person we decided to meet few people such that the person to whom we pass the news will spread it to all his friends. And those friends will pass it to other friends and so on. Your task is to find the number of people to be met by the organizers to spread the news.</p>

<p><strong>Caution:</strong> Large I/O</p>

<h3>Input</h3>
<p>First line of input is 't' - Test cases. Follwed by N, the number of peers in the testcase ( 0 to N-1 ). followed by the number of friend description 'e'. Following are 'e' descriptions of type "a b" denoting 'a' friends with 'b'.
If 'a' is friends with 'b' then 'b' is friends with 'a'.</p>

<h3>Output</h3>
<p>Output contains t line, the number of people, the organizers have to meet in person for each test case.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2

4
2
0 1
1 2

3
0

<strong>Output:</strong>
2
3</pre>

<h3>Explanation</h3>
<p>case 1 : 0 is friends with 1; 1 is friends with 2;  so if we pass the news to 0 &amp; 3, news will pass it to the entire N peers.</p>
<p>case 2 : no one is friends with any one. So we have to meet every one in person. </p>

<h3>Constraints</h3>
<p>
t = 10<br>
2 &lt;= N &lt;= 100000<br>
0 &lt;= e &lt;= N/2
</p>