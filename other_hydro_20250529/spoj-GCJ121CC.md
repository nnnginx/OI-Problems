<p>You own a factory with two assembly lines. The first assembly line makes boxes, and the second assembly line makes toys to put in those boxes. Each type of box goes with one type of toy and vice-versa.&nbsp;<br><br> At the beginning, you pick up a box from the first assembly line and a toy from the second assembly line. You then have a few options.</p>
<p># You can always throw out the box and pick up the next one.&nbsp;<br># You can always throw out the toy and pick up the next one.&nbsp;<br># If the box and toy are the same type, you can put the toy in the box, and send it out to customers.</p>
<p>You always pick boxes up in the order in which they are made, and similarly for toys. You know the order in which boxes and toys are made, and you want to plan out a strategy that will allow you to send as many boxed toys as possible to customers. <br><br><br>&nbsp;Warning: The two assembly lines make a lot of boxes and toys. However, they tend to make one kind of thing for a long period of time before switching.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases, T. T test cases follow.<br><br> Each test case begins with a line contains two integers N and M. It is followed by a line containing 2 * N integers a1, A1, a2, A2, ..., aN, AN, and another line containing 2 * M integers b1, B1, b2, B2, ..., bM, BM. <br><br> This means that the first assembly line will make a1 boxes of type A1, then a2 boxes of type A2, etc., until it finishes with aN boxes of type AN. Similarly, the second assembly will make b1 toys of type B1, followed by b2 toys of type B2, etc., until it finishes with bM toys of type BM. <br><br>&nbsp;A toy can be matched with a box if and only if they have the same type number.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is the case number (starting from 1), and y is the largest number of boxed toys that you can send out to customers.</p>
<h3>Limits</h3>
<p>1 �� T �� 100.<br> 1 �� ai, bi �� 10<sup>16</sup>.<br> 1 �� Ai, Bi �� 100.</p>
<p>1 �� N, M �� 100.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>
4<br>3 3<br>10 1 20 2 25 3<br>10 2 30 3 20 1<br>3 5<br>10 1 6 2 10 1<br>5 1 3 2 10 1 3 2 5 1<br>3 5<br>10 1 6 2 10 1<br>5 1 6 2 10 1 6 2 5 1<br>1 1<br>5000000 10<br>5000000 100<br><br><strong>Output:</strong><br><br>Case #1: 35<br>Case #2: 20<br>Case #3: 21<br>Case #4: 0<strong><br></strong>

</pre>