<p>Halum has been elected as the captain of his school's football team. To celebrate this, he is going to throw a party. Halum bought candies of <strong>N</strong> different flavors for the party. There are <strong>a<sub>i</sub></strong> number of candies of the <strong>i<sup>th</sup></strong> flavor where <strong>(1 ¡Ü i ¡Ü N)</strong>. To satisfy a guest he has to give him/her some positive number of candies of at least <strong>K</strong> different flavors. Otherwise the guest is not satisfied. Given this information now you have to find the maximum number of guests Halum can satisfy with the available candies.</p>
<h3>Input</h3>
<p>First line of the input contains an integer <strong>T (1 ¡Ü T ¡Ü 200)</strong>, denoting the number of test cases. <strong>T</strong> cases follow.<br> First line of each case contains two integers <strong>N</strong> and <strong>K</strong> <strong>(1 ¡Ü K ¡Ü N ¡Ü 1000)</strong>. <strong>N</strong> space separated integers <strong>a<sub>1</sub>, a<sub>2</sub>¡­ a<sub>N</sub></strong> follow in the next line <strong>(0 ¡Ü a<sub>i</sub> ¡Ü 10^9)</strong>. The <strong>i<sup>th</sup></strong> of these integers <strong>a<sub>i</sub></strong> denotes the number of candies of <strong>i<sup>th</sup></strong> flavor <strong>(1 ¡Ü i ¡Ü N)</strong>.</p>
<h3>Output</h3>
<p>For each case print one line containing "<strong>Case X: Y</strong>" (without the quotes) where <strong>X</strong> is the case number starting from <strong>1</strong> and <strong>Y</strong> is an integer denoting the maximum number of guests who can be satisfied.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 3
1 2 3
3 1
1 2 3
3 2		
3 2 4

<strong>Output:</strong>
Case 1: 1
Case 2: 6
Case 3: 4
</pre>