<p>As usual Popeye and brutus are fighting for olive, and suddenly a witch  appears and took popeye to magical land as brutus called that witch. In magical land, the witch with her magic make <strong>N</strong>(1&lt;=N&lt;=100) number of clones of popeye of different strength(0&lt;=Si&lt;=100) i.e each popeye can hold another popeyes above his head, and number of popeyes which can be hold will be  less than or equal to strength of popeye which is holding other popeyes.</p>
<p>Eg: Imagine there are three popeyes: the first has strength 2, the  second has strength 1 and the third has strength 1. We cannot put the  second and the third popeye simultaneously on the top of the first one. But the  second popeye can place directly on the top of the first one, and then  the third popeye directly on the top of the second one.We will call such construction of popeye a <strong>"Popeye-stack"</strong>.<br> <br> The witch want him to make <strong>Minimum</strong> number of popeye-stack and give her <strong>Maximum Height</strong> of popeye-stack from that arrangement, then only she release him from the magic and give him spinach to defeat brutus. Help popeye to get released from the magic of the witch.</p>
<h3>Input</h3>
<p>First line of Input contains no. of test cases T(T&lt;=1000). Each test case contain two lines: 1st line contains N (1&lt;=N&lt;=100)  and 2nd line contain N spaced Si (strength of N popoyes)  (0&lt;=Si&lt;=100)</p>
<h3>Output</h3>
<p>For each test case output a string "Case #i: " ("i" is test case number) followed by <strong>Minimum</strong> number of popeye-stack and <strong>Maximum Height</strong> of popeye-stack seperated by a space.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5<br>0 1 2 3 4 <br>9<br>0 1 0 2 0 1 1 2 10

<strong>Output:</strong>
Case #1: 1 5<br>Case #2: 3 4
</pre>