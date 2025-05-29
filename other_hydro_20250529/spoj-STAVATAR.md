<p><span style="font-size: small;">The charland nation has declared a war on all nations. <span style="font-size: small;">To defeat the charlord stavatar</span> has to meet his previous stavatar form(stoku) in the char temple for some guidance. To open the char temple one has to enter two passwords simulatenously.</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">The charland benders knew that this would happen some day and they modified the password to char temple with a special charland bending technique.</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">The special charland bending technique is swapping the characters between two strings(passwords) of length N from L to R in their respective positions(Inclusive).</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">for example a typical special charland bending technique on the below strings(L=2 and R=4)</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"><code>abcdef ghijkl</code></span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">transforms them to</span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;"><code> abijkf ghcdel </code></span></p>
<p><span style="font-size: small;">now the stavatar has successfuly robbed the records(scroles) of these modifications to the passwords. but a little bit confused on how to obtain the original passwords. can you help him ??<br></span></p>
<p><span style="font-size: small;"> </span></p>
<h3><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">First line contains&nbsp; the length of two strings(N) and then the next two lines contain the two modified passwords of length N each. and then in the next line <span style="font-size: small;">M -</span> the number of bendings applied to get the given passwords. the next M lines consist of two space separated integers L and R.</span></p>
<p><span style="font-size: small;"> </span></p>
<h3><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">print the two passwords in two lines.</span></p>
<h3><span style="font-size: small;">Constraints</span></h3>
<pre><span style="font-size: small;">1 &lt;= N &lt;= 10<sup>6</sup><br>1 &lt;= M &lt;= 10<sup>6</sup><br>0 &lt;= L &lt;= R &lt; N<br>a password can contain any printable character except a newline(ofcourse). the printable characters can represented as<code><br><img src="file://WrSp8Dz8.png" alt="the printable characters representation." width="690" height="52"></code></span></pre>
<p><span style="font-size: small;"> </span></p>
<h3><span style="font-size: small;">Example</span></h3>
<p><span style="font-size: small;"> </span></p>
<pre><span style="font-size: small;"><strong>Input:</strong><br>6<br>abcdef<br>ghijkl<br>4<br>2 4<br>1 3<br>4 4<br>4 5<br><br><strong>Output:</strong>
ahcdkl<br>gbijef<br><br><pre><span style="font-size: small;">Note: To be presice the representation of output is <code>"ahcdkl\ngbijef\n"</code></span><br>My Best: C++: 0.35s, python2.7: 12.57, pypy: 6.27.<br></pre>
</span></pre>