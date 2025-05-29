<p><span style="font-size: small;">Reference:: The Hobbit : Desolation of Smaug<br> <a href="http://en.wikipedia.org/wiki/The_Hobbit:_The_Desolation_of_Smaug">The_Hobbit:_The_Desolation_of_Smaug</a></span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> J. R. R. Tolkien decided to make Thorin Oakenshield¡¯s task more difficult.   This time he was given an infinite number of keys represented by a small   string. The hidden entrance has a lot of keyholes side by side represented by   one long string. The key fits only into a slit that matches it completely.   Oakenshield does not know how many keys he would require and which all   keyholes he will have to try out. So if there are <strong>n</strong> keyholes where the key   fits, he might need any number of keys between <strong>1 to n</strong> (both inclusive).   Moreover he does not know which keyholes among the ones where the keys fit, he   will have to use. All he knows is that there is a unique way to open the door.   Trying out each configuration takes <strong>1</strong> second. The last light of Durin¡¯s day   does not last long and will have to try out all possibilities before it goes.   He wants you to find out how long, in the worst case, it will take for him to   try out all possibilities.</span></p>
<p><span style="font-size: small;"> Since the answers may be huge, output it modulo <strong>1000000007</strong>.   If there are no keyholes where the key fits, output <strong>0</strong>. </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> First line containing a string representing the key.   Second line containing a string representing the keyholes. </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> Single line containing an integer for the required answer. </span></p>
<h3><span style="font-size: small;">Notes:</span></h3>
<p><span style="font-size: small;"> 1. Key fits into a keyhole at index <strong>i</strong> if key is a substring of keyhole string   at index <strong>i</strong>.<br> 2. If there are two overlapping keyholes where the key may fit, you cannot   insert a key in both simultaneously </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 1 ¡Ü key ¡Ü 10^4<br> 1 ¡Ü keyholes ¡Ü 5*(10^5)<br></strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">c
a	</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">0</span></pre>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">aba
abababa</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">4</span></pre>
<h3><span style="font-size: small;">Explanation:</span></h3>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Explanation for Test Case #1:<br></strong> The key fits into keyholes at positions {1, 3, 5}<br> If he requires only 1 key he may put them at {1} or {3} or {5} = 3 seconds.<br> If he required 2 keys, he may put them at {1,5} = 1 second.<br> Total = 1+3 = 4 seconds.<br> He cannot use 3 keys without overlapping them.</span></p>
<p><span style="font-size: small;"><strong> Explanation for Test Case #2:<br></strong> There is no slit where the key fits hence 0 seconds.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Vidit Gupta</strong></span></p>