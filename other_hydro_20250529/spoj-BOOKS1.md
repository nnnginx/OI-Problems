<p>Before the invention of book-printing, it was very hard to make a copy of a book. All the contents had to be re-written by hand by so called <i>scribers</i>. The scriber had been given a book and after several months he finished its copy. One of the most famous scribers lived in the 15th century and his name was Xaverius Endricus Remius Ontius Xendrianus (<i>Xerox</i>). Anyway, the work was very annoying and boring. And the only way to speed it up was to hire more scribers.</p>

<p>
Once upon a time, there was a theater ensemble that wanted to play famous Antique Tragedies. The scripts of these plays were divided into many books and actors needed more copies of them, of course. So they hired many scribers to make copies of these books. Imagine you have <var>m</var> books (numbered <var>1, 2 ... m</var>) that may have different number of pages (<var>p<sub>1</sub>, p<sub>2</sub> ... p<sub>m</sub></var>) and you want to make one copy of each of them. Your task is to divide these books among <var>k</var> scribes, <var>k &lt;= m</var>. Each book can be assigned to a single scriber only, and every scriber must get a continuous sequence of books. That means, there exists an increasing succession of numbers <var>0 = b<sub>0</sub> &lt; b<sub>1</sub> &lt; b<sub>2</sub>, ... &lt; b<sub>k-1</sub> &lt;= b<sub>k</sub> = m</var> such that <var>i</var>-th scriber gets a sequence of books with numbers between <var>b<sub>i-1</sub>+1</var> and <var>b<sub>i</sub></var>. The time needed to make a copy of all the books is determined by the scriber who was assigned the most work. Therefore, our goal is to minimize the maximum number of pages assigned to a single scriber. Your task is to find the optimal assignment.</p>

<h3>Input</h3>

<p>The input consists of <var>N</var> cases (equal to about 200). The first line of the input contains only positive integer <var>N</var>. Then follow the cases. Each case consists of exactly two lines. At the first line, there are two integers <var>m</var> and <var>k</var>, <var>1 &lt;= k &lt;= m &lt;= 500</var>. At the second line, there are integers <var>p<sub>1</sub>, p<sub>2</sub>, ... p<sub>m</sub></var> separated by spaces. All these values are positive and less than 10000000.</p>

<h3>Output</h3>
<p>For each case, print exactly one line. The line must contain the input succession <var>p<sub>1</sub>, p<sub>2</sub>, ... p<sub>m</sub></var> divided into exactly <var>k</var> parts such that the maximum sum of a single part should be as small as possible. Use the slash character ('<tt>/</tt>') to separate the parts. There must be exactly one space character between any two successive numbers and between the number and the slash.</p>

<p>If there is more than one solution, print the one that minimizes the work
assigned to the first scriber, then to the second scriber etc. But each
scriber must be assigned at least one book.</p>

<h3>Example</h3>

<pre><b>Sample input:</b>
2
9 3
100 200 300 400 500 600 700 800 900
5 4
100 100 100 100 100

<b>Sample output:</b>
100 200 300 400 500 / 600 700 / 800 900
100 / 100 / 100 / 100 100</pre>