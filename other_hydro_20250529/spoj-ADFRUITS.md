<p>The company "21st Century Fruits" has specialized in creating new sorts of fruits by transferring genes from one fruit into the genome of another one. Most times this method doesn't work, but sometimes, in very rare cases, a new fruit emerges that tastes like a mixture between both of them.</p>
<p>A big topic of discussion inside the company is "How should the new creations be called?" A mixture between an apple and a pear could be called an apple-pear, of course, but this doesn't sound very interesting. The boss finally decides to use the shortest string that contains both names of the original fruits as sub-strings as the new name. For instance, "applear" contains "apple" and "pear" (APPLEar and apPlEAR), and there is no shorter string that has the same property. <br> A combination of a cranberry and a boysenberry would therefore be called a "boysecranberry" or a "craboysenberry", for example.</p>
<p>Your job is to write a program that computes such a shortest name for a combination of two given fruits. Your algorithm should be efficient, otherwise it is unlikely that it will execute in the alloted time for long fruit names.</p>
<h3>Input Specification</h3>
<p>Each line of the input file contains two strings that represent the names of the fruits that should be combined. All names have a maximum length of 100 and only consist of alphabetic characters.<br> Input is terminated by end of file.</p>
<h3>Output Specification</h3>
<p>For each test case, output the shortest name of the resulting fruit on one line. If more than one shortest name is possible, any one is acceptable.</p>
<h3>Sample Input</h3>
<pre>apple peach
ananas banana
pear peach
</pre>
<h3>Sample Output</h3>
<pre>appleach
bananas
pearch
</pre>