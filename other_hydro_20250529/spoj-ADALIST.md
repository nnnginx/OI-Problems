<p>Ada the Ladybug has a TODO-list (containing only numbers - for simplicity). She is still doing something, so she sometimes erases <strong>k</strong><sup>th</sup> number, sometimes she inserts something on <strong>k</strong><sup>th</sup> position and sometime she asks for <strong>k</strong><sup>th</sup> number.</p>
<p>Sadly, she is now searching for a work at position <strong>k</strong> so she doesn't have time to do this herself. Can you help her?</p>
<h3>Input</h3>
<p>The first line will contain <strong>0 &lt; N ¡Ü 10<sup>5</sup>,0 &lt; Q &lt;             5*10<sup>5</sup></strong>, the number of elements in TODO-list and         number of queries.</p>
<p>Then a line with <strong>N</strong> numbers follows. Each number         <strong>0 ¡Ü A<sub>k</sub> ¡Ü 10<sup>9</sup></strong> means         <strong>k</strong><sup>th</sup> number in her TODO-list.</p>
<p>Afterward, <strong>Q</strong> lines follow, each beginning with number <strong>1 ¡Ü a     ¡Ü 3</strong></p>
<p>1 <strong>k x</strong> means that you will add number <strong>x</strong> to position <strong>k</strong></p>
<p>2 <strong>k</strong> means that you will erase number from position <strong>k</strong></p>
<p>3 <strong>k</strong> means that you will print number from position <strong>k</strong></p>
<p>For all queries, it is true that <strong>1 ¡Ü k ¡Ü #SizeOfList</strong>, <strong>0     ¡Ü x ¡Ü 10<sup>9</sup></strong> (for query <strong>1</strong>, it can be also put to position <strong>#SizeOfList + 1</strong>)</p>
<p>You will never get query of type <strong> 2 </strong> or <strong> 3 </strong> if the list is empty</p>
<h3>Output</h3>
<p>For each query of type <strong>3</strong>, print <strong>k</strong><sup>th</sup> numbers</p>
<h3>Example Input</h3>
<pre>6 10
1 2 4 8 16 32
3 4
1 1 7
3 2
2 2
2 2
3 2
1 6 666
3 6
2 1
3 1

</pre>
<h3>Example Output</h3>
<pre>8
1
4
666
4
</pre>
<h3>Queries explanations</h3>
<pre>1 2 4 <span style="color: red;"><strong>8</strong></span> 16 32
7 1 2 4 8 16 32
7 <span style="color: red;"><strong>1</strong></span> 2 4 8 16 32
7 2 4 8 16 32
7 4 8 16 32
7 <span style="color: red;"><strong>4</strong></span> 8 16 32
7 4 8 16 32 666
7 4 8 16 32 <span style="color: red;"><strong>666</strong></span>
4 8 16 32 666
<span style="color: red;"><strong>4</strong></span> 8 16 32 666

</pre>