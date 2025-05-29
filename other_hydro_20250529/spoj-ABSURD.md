<p>Surely you know that supermarkets, shopping centres, and indeed all kind of vendors seem to have fallen in love with the digit <em>9</em>, for that digit occurs most often in the price of a product, preferably at the least significant positions. Your favourite chocolate bar might cost <em>99</em> cents, just right to be able to advertise that it costs less than <em>1</em> euro. Your new bicycle might cost <em>499.98</em> euros, which, of course, is less than <em>500</em> euros.</p>
<p>While such comparisons are mathematically sound, they seem to impose a certain amount of stupidity on the customer. Moreover, who wants to carry home those annoying small coins you get back as change?</p>
<p>Fortunately, the FIFA has not adopted this weird pricing scheme: a ticket for the final in the first category for example costs <em>900</em> dollar, in the second category <em>600</em> dollar and in the third category <em>400</em> dollar. These prices may only be regarded weird for other reasons.</p>
<p>We want to distinguish between <strong>absurd</strong> prices like <em>99</em> cents, <em>499.98</em> euros, etc. and normal prices. To measure the absurdity of a positive integer, do the following:</p>
<ul>
<li>Eliminate all trailing zeros, i.e., those in the least significant positions, from the number. You now have a positive integer, say <em>x</em>, with a non-zero digit <em>d</em> at its end.</li>
<li>Count the number of digits, say <em>a</em>, of the number <em>x</em>.</li>
<li>if <em>d=5</em> the absurdity of the number is <em>2 * a - 1</em></li>
<li>otherwise, the absurdity of the number is <em>2 * a</em></li>
</ul>
<p>For example, the absurdity of <em>350</em> is <em>3</em> and the absurdity of <em>900900</em> is <em>8</em>. Using the measure of absurdity, we can define what we call an absurd price: A price <em>c</em> is absurd if and only if the closed interval [<em>0.95 * c,1.05 * c</em>] contains an integer <em>e</em> such that the absurdity of <em>e</em> is less than the absurdity of <em>c</em>. Given a price in cents, go ahead and tell whether it is absurd!</p>
<h3>Input</h3>
<p>The first line of the input consists of the number <em>t</em> of test cases to follow. Each test case is specified by one line containing an integer <em>c</em>. You may assume that <em>1 ¡Ü c ¡Ü 10<sup>9</sup></em>.</p>
<h3>Output</h3>
<p>For each test case output if <em>c</em> is absurd or not. Adhere to the format shown in the sample output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
99
49998
90000
970000000

<strong>Output:</strong>
absurd
absurd
not absurd
absurd
</pre>