<p>Sam and Dean fight the supernatural creatures to protect the humans. Now they have come across a creature called the Vedala, which are always found in pairs. Each vedala can be represented by a polynomial. Both the Vedalas need to be killed at once or else they can't be killed. They can be killed only by using the product of the two polynomials representing the two Vedala. Help Sam and Dean find the product of the polynomials fast, so they can do thier work.&nbsp;</p>

<h3>Input</h3>
<p>First line contains an integer&nbsp;<strong>T (¡Ü 10)</strong>, number of test cases.</p>
<p>Each test case will have&nbsp;<strong>n (n ¡Ü 10000)</strong>, maximum degree of the polynomials on the first line.&nbsp;</p>
<p>Next two lines will have n+1 space separated integers each representing the coeffiecients of first and second polynomials respectively.</p>
<p>All input coefficients values are <strong>&lt;=1000</strong>.</p>

<h3>Output</h3>
<p>For each test case ouput a line of 2n space seperated integers indicating coefficients of the polynomial created after multiplication.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
1 2 3
3 2 1
2
1 0 1
2 1 0

<strong>Output:</strong>
3 8 14 8 3
2 1 2 1 0</pre>

<h3>Explaination</h3>
<p>1st test case n=2, the polynomials are x^2 + 2x + 3 and 3x^2 + 2x + 1.</p>
<p>On multiplying we get 3x^4 + 8x^3 + 14x^2 + 8x + 3 and hence the answer is 3 8 14 8 3.</p>

<p>2nd test case n=2, the polynomials are x^2 + 1 and 2x^2 + x.&nbsp;</p>
<p>On multiplying we get 2x^4 + x^3 + 2x^2 + x and hence the answer is 2 1 2 1 0.&nbsp;</p>