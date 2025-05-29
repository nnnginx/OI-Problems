<p>As you might already know, Ada the Ladybug has a huge TODO-list. Sometimes she inserts a new job into her TODO-list and sometimes she is wondering whether there is a job (in her TODO-list), which she wants to do now. She doesn't require the whole job to be there, perhaps just a part of it.</p>
<p>Can you create a program which would serve her? That means it either inserts a new job into her TODO-list or answers whether there exists a word (in her TODO-list) which is a substring of given word.</p>
<h3>Input</h3>
<p>The first line of input containts  <strong>Q</strong>, the number of queries.</p>
<p>The next <strong>Q</strong> lines contains a number <strong>0 ¡Ü t  ¡Ü 1</strong> and nonempty string <strong>s</strong>. If <strong>t</strong> is equal to <strong>0</strong> then it is inserion query, otherwise it is question query. <strong>s</strong> consists of lowercase characters only.</p>
<p>The sum of lengths of queries of both types doesn't exceed <strong>10<sup>6</sup></strong> (that means the total sum of lengths of strings will be at most <strong>2*10<sup>6</sup></strong>)</p>
<h3>Output</h3>
<p>For each query of type <strong>1</strong>, print either <strong>YES</strong>, if there is already a substring in the TODO-list and <strong>NO</strong> otherwise.</p>
<h3>Example Input</h3>
<pre>12
0 cat
1 dogville
0 dog
1 dogville
1 gooutwithcat
1 gooutwithcrocodile
1 fancyconcatenation
0 crocodile
1 lacoste
1 gooutwithcrocodile
1 catalanreferendum
1 rocodile
</pre>
<h3>Example Output</h3>
<pre>NO
YES
YES
NO
YES
NO
YES
YES
NO
</pre>