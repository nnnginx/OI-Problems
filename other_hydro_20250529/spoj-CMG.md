<p>One day after storm mina went to pick up mangoes in the garden with a basket. She began to pick up mangoes from the garden. And if she wants, she can throw away the last picked up mango from the basket. In this way, mina kept picking up mangoes. She brought you with her to keep track of the biggest size of mango in the basket at that time. At any moment Mina can ask you about the biggest size of mango. Your job is to help Mina.</p>
<p>Since you are a good programmer, so you write a program by which you are easily able to answer the question of Mina.</p>
<p>During picking up mangoes, Mina can have 3 types of question/instruction for you.</p>
<p>1.&nbsp; Type 1: put an ¡®x¡¯ size mango in the basket, which is picked up form garden.</p>
<p>2.&nbsp; Type 2: Throw out last picked up mango. (There can be consecutive throw out operation. )</p>
<p>3.&nbsp; Type 3: Ask for the biggest mango size in the basket at that moment.</p>
<h3>Input</h3>
<p>The first line contains a positive integer <strong>T</strong>, number of test case. In the following each case start with a positive integer N, which is number of question/operation Mina will ask during picking up mangoes. Next N lines will contain 3 types of operations (A, R, Q). A x, here x is picked up mango size. R, throw out last picked up mango from basket. Q Find out the biggest size mango.</p>
<h3>Output</h3>
<p>For each case, first print the case number and print the answer of Mina¡¯s question. Whenever the basket is empty, then Mina¡¯s question¡¯s answer will be ¡°Empty¡±.</p>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;">Constraints</span></strong></p>
<ul>
<li>1&lt;=T&lt;=25<strong>&nbsp;</strong></li>
<li>1&lt;=N&lt;=100000<strong>&nbsp;</strong></li>
<li>1&lt;=x&lt;=100000<strong>&nbsp;</strong></li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2</p><p>6</p><p>A 10</p><p>A 5</p><p>Q</p><p>A 100</p><p>R</p><p>Q</p><p>6</p><p>A 5</p><p>Q</p><p>R</p><p>Q</p><p>R</p>R

<strong>Output:</strong>
<p>Case 1:<br>10<br>10<br>Case 2:<br>5<br>Empty</p></pre>