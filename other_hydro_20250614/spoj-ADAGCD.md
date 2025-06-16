<p>Ada the Ladybug got interesting homework. She had to count gcd of a few numbers. As she is a great mathematician, she done it in meanwhile (in fact, she submited it during the class it was assigned in). The teacher was impressed so he gave Ada a bonus homework (for bonus points). It is same as previous one with a little difference - there are bigger numbers.</p>
<p>Since the number are too large to be written as numbers, they are written as product of lesser numbers. Find their gcd.</p>
<h3>Input</h3>
<p>The first line of input consists of <strong> 2 ¡Ü N ¡Ü 10<sup>6</sup></strong>, the number of numbers for which Ada wants to find their gcd.</p>
<p>Each of the next <strong>N</strong> lines contains an integer <strong>1 ¡Ü M<sub>i</sub> &lt;  10<sup>6</sup></strong> followed by <strong>M<sub>i</sub></strong> integers, <strong>1 ¡Ü A<sub>j</sub> ¡Ü 10<sup>7</sup></strong>, the numbers whose product is the <strong>i<sup>th</sup></strong> number.</p>
<p>The sum of all <strong>M<sub>i</sub></strong> won't exceed <strong>10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>Print the <strong>gcd</strong> on a single line. Since this number might be pretty big, output it modulo <strong>10<sup>9</sup>+7</strong> (<strong>1000000007</strong>)</p>
<h3>Example Input 1</h3>
<pre>3
4 1 2 3 4
1 36
2 6 5
</pre>
<h3>Example Output 1</h3>
<pre>6
</pre>
<h3>Example Input 2</h3>
<pre>2
11 1 2 3 4 5 6 7 8 9 10 11
2 1024 15 
</pre>
<h3>Example Output 2</h3>
<pre>3840
</pre>