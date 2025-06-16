<p style="text-align: left;">In this problem, you¡¯ll be helping a little bookworm, Kuchu.</p>
<p style="text-align: left;">Recently ¡°Omuk book shop¡± has announced a huge sale on various books. Being a bookworm, Kuchu could not miss this opportunity and went there immediately!</p>
<p style="text-align: left;">When reached there, she noticed that conditions of the sale are:</p>
<ol style="text-align: left;">
<li>One must buy exactly B books to get the discount.</li>
<li>Maximum number of pages in any book is no more than 100.</li>
</ol><ol style="text-align: left;"> </ol>
<p style="text-align: left;">As she wants to read as much as possible, Kuchu wants to get maximum number of pages satisfying the conditions above. Now she is wondering if there are N books in the store, how many different ways are there to choose exactly B books so that the number of pages is maximum possible.</p>
<p style="text-align: left;">Not all books are interesting to little kids, so you are given two information about each book-</p>
<ol style="text-align: left;">
<li>Number of pages P.</li>
<li style="text-align: left;">Interest value V. V is 1 if the book is interesting for kids and 0 otherwise.</li>
</ol>
<h3 style="text-align: left;">Input</h3>
<p>First line contains an integer T, the number of test cases.</p>
<p>For each test case, the first line contains two integers N and B as mentioned above. Next N lines contain two integers each P<sub>i</sub> and V<sub>i</sub>, number of pages and interest factor of ith book.</p>
<p>1 ¡Ü T ¡Ü 25</p>
<p>1 ¡Ü N ¡Ü 100,000</p>
<p>1 ¡Ü B ¡Ü N</p>
<p>1 ¡Ü P<sub>i</sub> ¡Ü 100</p>
<p>0 ¡Ü V<sub>i</sub> ¡Ü 1</p>
<h3 style="text-align: left;">Output</h3>
<p>For each test case, print one integer, the number of different ways to choose exactly B <strong>interesting books</strong> from those N books so that the number of pages is maximum possible. As result can be pretty large, print it modulo <strong>1,000,000,007 (10^9+7)</strong>.</p>
<h3 style="text-align: left;">Example</h3>
<pre style="text-align: left;"><strong>Input:</strong>
<p>2<br>2 1<br>2 0<br>3 0<br>5 3<br>10 0<br>5 1<br>2 1<br>2 1<br>2 1</p><strong>Output:</strong>
<p>0<br>3</p></pre>