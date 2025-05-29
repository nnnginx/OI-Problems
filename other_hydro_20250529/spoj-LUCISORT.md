<p>Lucifer is as bored as G-One after the defeat of Raone. he has no comuter game to play.</p>
<p>He Like g-One started reading books and Unlike G-One he bought a Big book shelf and lots of books</p>
<p>He labled all books with serial numbers.(All books have separate serial numbers).</p>
<p>&nbsp;</p>
<p>He invites his friends and small kids to home and allows them to read books. But the problem is everyone replaces the books anywhere on the shelf.</p>
<p>&nbsp;</p>
<p>At the end of the day Lucifer has to sort all the books in increasing order of serial number on the shelf from left to right.</p>
<p>The problem is He knows just one way of sorting called LUCIFER SORT.</p>
<p>&nbsp;</p>
<p>He can pick a book from anywhere on the shelf but can Replace it only in the center of the remaining books.</p>
<p>For eg. of the books are in order</p>
<p>2 1 3 4 5 6</p>
<p>The steps of sorting are</p>
<p>1 3 4 2 5 6 &nbsp;- &nbsp;Pick 2 and place between between 4 &amp; 5 in (1 3 4 5 6)</p>
<p>1 4 2 3 5 6 &nbsp;- &nbsp;Pick 3 and place between between 2 &amp; 5 in (1 4 2 5 6)</p>
<p>1 2 3 4 5 6 &nbsp;- &nbsp;Pick 4 and place between between 3 &amp; 5 in (1 2 3 5 6)</p>
<p>&nbsp;</p>
<p>Assuming positions are numbered from 1 to N.</p>
<p>While Replacing if number of books left is even then it is put back between n/2 and n/2+1 position.</p>
<p>if the books left are odd it is put back between (n+1)/2 and (n+1)/2+1 position.</p>
<p>&nbsp;</p>
<p>Since the number of books are large , he needs your help to tell me number of steps he needs to sort the shelf.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>first line contains number of shelves 'svs'</p>
<p>For each shelf there are 2 lines.</p>
<p>first line will have number of books 'bks'</p>
<p>second line will have the serial number of the books at the end of the day.</p>
<h3>Output</h3>
<p>Single line telling how many books he needs to remove and replace.</p>
<p>If there is no way he can sort the books by this process Print "YOU ARE DOOMED" without the quotes.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre>3</pre>
<pre>6</pre>
<pre>1 2 3 4 5 6</pre>
<pre>6</pre>
<pre>2 1 3 4 5 6</pre>
<pre>6</pre>
<pre>6 5 4 3 2 1

<strong>Output:</strong>

</pre>
<pre>0</pre>
<pre>3</pre>
<pre>6</pre>
<pre><pre style="font-size: 13px; text-align: left; color: #000020; background-color: #f6f9e0;">All the values will be in the range [0, 10^7] <br>number of test cases &lt;=100.</pre>
</pre>