<pre><i>A perfect rhyme is not a crime,
it is something that exceeds time, 
a bit of science, a piece of art, 
soft as a pillow, sharp as a dart.</i></pre>
<p>Everyone tried it, but only few chosen ones succeeded. It is a hard task with an unclear path, but a famous end ¨C should you reach it. Many compare it to finding the Holy Grail, or even to finding Waldo. The task is to find a perfect rhyme.</p>

<h3>Problem specification</h3>

<p>Given is a wordlist <b>L</b>, and a word <b>w</b>. Your task is to find a word in <b>L</b> that forms a perfect rhyme with <b>w</b>. This word <b>u</b> is uniquely determined by these properties:</p>
<div align="justify">
       <ul>
               <li>
               It is in <b>L</b>. 
               </li><li>
               It is different from <b>w</b>.
               </li><li>
               Their common suffix is as long as possible. 
               </li><li>
               Out of all words that satisfy the previous points, <b>u</b> is the lexicographically smallest one.
               </li>
       </ul>
</div>
<h3>Notes</h3>
<p>A prefix of a word is any string that can be obtained by repeatedly deleting the last letter of the word. Similarly, a suffix of a word is any string that can be obtained by repeatedly deleting the first letter of the word. 

</p><p>For example, consider the word <i>different</i>. 

</p><p>This word is both its own prefix and suffix. Its longest other prefix is <i>differen</i>, and its longest other suffix is <i>ifferent</i>. The string <i>rent</i> is its yet another, even shorter suffix. The strings <i>eent</i> and <i>iffe</i> are neither prefixes nor suffixes of the word <i>different</i>. 

</p><p>Let <b>u</b> and <b>v</b> be two different words. We say that <b>u</b> is lexicographically smaller than <b>v</b> if either <b>u</b> is a prefix of <b>v</b>, or if <i>i</i> is the first position where they differ, and the <i>i</i>-th letter of <b>u</b> is earlier in the alphabet than the <i>i</i>-th letter of <b>v</b>. 

</p><p>For example, <i>dog</i> is smaller than <i>dogs</i>, which is smaller than <i>dragon</i> (because <i>o</i> is less than <i>r</i>). 

</p><h3>Input specification</h3>

<p>The input file consists of two parts. The first part contains the wordlist <b>L</b>, one word per line. Each word consists of lowercase English letters only, and no two words are equal. 

</p><p>The first part is terminated by an empty line.

</p><p>The second part follows, with one query word <b>w</b> per line.

</p><p>You may assume that in either part of the input, the length of a word will be no more than 30. And the number of words in each part of the input will be no more than 250000. The input file will be less than 5MB. </p>

<h3>Output specification</h3>

<p>For each query in the input file output a single line with its perfect rhyme. The output must be in lowercase.</p>

<h3>Example</h3>
<pre><b>input:</b>
perfect
rhyme
crime
time

crime
rhyme

<b>output:</b>
time
crime
</pre>
<p>In the second test case, there were two candidates that had an equally long common suffix (crime and time), the lexicographically smaller one was chosen.</p>

<b>Warning: large input/output data, be careful with certain languages</b>