<p><span style="font-size: small;"> Swayamvara, in ancient India, was a practice of choosing a husband, from a   list of suitors by a girl of marriageable age.</span></p>
<p><span style="font-size: small;"> It is the swayamvara of gossip queen of IIIT, Akshata. Now, Akshata is always   interested in knowing the stability of the relationships among various   students of IIIT. Nowadays she is very busy in her swayamvara��s preparation   and is not able to update herself about the latest gossips. As you know she is   the gossip queen. She would love if someone could do her a favor and collect   answers of her questions about relationships in IIIT. It might increase the   collector��s chance of getting selected for marriage.</span></p>
<p><span style="font-size: small;"> Before starting preparations for the swayamvara, Akshata used to maintain   notes about the relationships in IIIT and knew all about them. So she thought   she can help you by providing the notes.</span></p>
<p><span style="font-size: small;"> There are various ways in which two people can be acquaintances :</span></p>
<ol>
<li><span style="font-size: small;">If <strong>A</strong> and <strong>B</strong> are in a relationship, then <strong>A</strong> and <strong>B</strong> are acquaintances of each   other.</span></li>
<li><span style="font-size: small;"> If <strong>A</strong> and <strong>B</strong> are acquaintances of each other and <strong>B</strong> and <strong>C</strong> are acquaintances of   each other, then<strong> A</strong> and <strong>C</strong> are also acquaintances of each other. </span></li>
</ol>
<p><span style="font-size: small;">In Akshata's notes, a relationship between <strong>person1</strong> and <strong>person2</strong> is represented   as <strong>"person1 person2"</strong>. The Queen's questions are also special. </span></p>
<p><span style="font-size: small;">There are two types of questions: </span></p>
<ol>
<li><span style="font-size: small;">First type of query is whether two people, say <strong>A</strong> and <strong>B</strong>, still remain each   others�� acquaintances even if two people, say <strong>C</strong> and <strong>D</strong>, break-up and end their   relationship.</span></li>
<li><span style="font-size: small;"> Second type of query is whether two people, say <strong>A</strong> and <strong>B</strong>, still remain   acquaintances even if a person, say <strong>C</strong>, leaves the college (It��s obvious that   before leaving college, <strong>C</strong> ends all his/her relationships).</span></li>
</ol>
<p><span style="font-size: small;"><br></span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> First line of the input contains two integers, <strong>N</strong> and <strong>M</strong> where <strong>N</strong> represents the   number of people in IIIT and <strong>M</strong> represents the number of relationships in   Akshata��s notes.</span></p>
<p><span style="font-size: small;">The next <strong>M</strong> lines contain <strong>2</strong> strings each, containing the names of <strong>2</strong> people who   are in a relationship.</span></p>
<p><span style="font-size: small;"> Next line contains a single integer <strong>Q</strong>, which represents the number of   questions asked by the Queen. Each of the next<strong> Q</strong> lines represents a query. For   every query first integer represents the query type.</span></p>
<p><span style="font-size: small;"> If the query type is <strong>1</strong> then it is followed by four strings in the same line,   representing <strong>A B C and D</strong>. you have to output <strong>"STABLE"</strong> if<strong> A and B</strong> remain   acquaintance of each other even if <strong>C and D</strong> break up and <strong>"NOT STABLE"</strong> otherwise.</span></p>
<p><span style="font-size: small;">If the query type is <strong>2</strong> then it is followed by three strings in the same line,   representing<strong> A B and C</strong>. You have to output <strong>"STABLE"</strong> if <strong>A and B</strong> remain   acquaintances even if <strong>C</strong> leaves college otherwise output <strong>"NOT STABLE"</strong>. (All   quotes for clarity) </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> For every query output <strong>"STABLE"</strong> or <strong>"NOT STABLE"</strong> without quotes. </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 1 �� N �� 10000<br> 1 �� M �� 50000<br> 1 �� Q �� 10000<br> Size of all strings will be less than 50 characters.<br></strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">3 2
Person1 Person2
Person1 Person3
2
2 Person2 Person3 Person1
1 Person1 Person2 Person1 Person3</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">NOT STABLE
STABLE</span></pre>
<h3><span style="font-size: small;">Explanation:</span></h3>
<p><span style="font-size: small;"> Person1 is in a relationship with Person2 and Person1 is also in a relation   with Person3. So Person3 and Person2 are acquaintance.<br> First Query: <br> But Person2 and Person3 are acquaintance of each other only because of   person1, if person1 leaves the college, then Person2 and Person3 are also not   acquaintance of each other.<br> Second Query: <br> Person1 will remain being acquaintance of Person2 even if Person1 breaks-up   with Person3.</span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">17 18
Person1 Person2
Person1 Person4
Person2 Person4
Person4 Person6
Person2 Person6
Person2 Person3
Person3 Person5
Person1 Person7
Person7 Person8
Person7 Person9
Person7 Person10
Person9 Person12
Person8 Person12
Person8 Person11
Person12 Person13
Person14 Person15
Person15 Person16
Person16 Person17
8
2 Person1 Person14 Person7
2 Person1 Person2 Person2
1 Person1 Person14 Person2 Person4
1 Person5 Person13 Person1 Person2
1 Person6 Person2 Person1 Person4
1 Person13 Person6 Person7 Person8
2 Person13 Person6 Person7
2 Person13 Person6 Person8
2 Person13 Person8 Person7</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">NOT STABLE
NOT STABLE
NOT STABLE
STABLE
STABLE
STABLE
NOT STABLE
STABLE</span></pre>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Mayank Natani</strong></span></p>