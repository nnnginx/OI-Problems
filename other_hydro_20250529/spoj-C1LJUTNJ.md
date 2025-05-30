<p>Children in a kindergarten have received a large sack containing M candies. It has been decided that the candies are to be distributed among N children.</p>
<p>Each child has stated the number of candies that it wants. If a child isn��t given the amount of candy it wants, it will get angry. In fact it��ll get angrier for each candy it is deprived of. Some speculate that it��s anger will be equal to the square of the number of candy it is deprived of. For instance, if Mirko states that he wants 32 candies but receives only 29, he would be missing 3 candies, so his anger would be equal to 9.</p>
<p>Unfortunately, there is an insufficient amount of candy to satisfy all children. Therefore, the candies should be distributed in such a way that the sum of the children��s anger is minimal.</p>
<h3>Input</h3>
<p>The first line contains two integers, M (1 �� M �� 2.10<sup>9</sup>) and N (1 �� N �� 100 000).</p>
<p>The following N lines contain integers (one per line) which represent the wishes of the children. Those numbers are all strictly less than 2.10<sup>9</sup>, and their sum always exceeds M.</p>
<h3>Output</h3>
<p>The first and only line of output must contain the minimum sum of the children��s anger.</p>
<p>Note: The test cases will ensure that the result fits in a 64-bit unsigned integer: int64 in Pascal, long long in C/C++, long in Java.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5 3 <br>1 <br>3 <br>2<br><strong>Output:</strong><br>1<strong><br><br>Input:</strong><br>10 4<br>4<br>5<br>2<br>3<strong><br><br>Output:</strong><br>4</pre>