<p>
Weird Wally's Wireless Widgets, Inc. manufactures an eclectic assortment
of small, wireless, network capable devices, ranging from dog collars,
to pencils, to fishing
bobbers. All these devices have very small memories.
Encryption algorithms like Rijndael, the candidate for the Advanced
Encryption Standard (AES) are demonstrably secure but they don't fit 
in such a tiny memory. In order to provide some security for 
transmissions to and from the devices, WWWW uses the following algorithm,
which you are to implement.
</p>

<p>
Encrypting a message requires three integer keys, <i>k<sub>1</sub></i>,

<i>k<sub>2</sub></i>, and <i>k<sub>3</sub></i>. The letters [a-i] form
one group, [j-r] a second group, and everything else ([s-z] and underscore) the
third group. Within each group the letters are rotated <i>left</i> by
<i>k<sub>i</sub></i> positions in the message.
Each group is rotated independently
of the other two.  Decrypting the message means doing
a <i>right</i> rotation 
by <i>k<sub>i</sub></i> positions within each group.

</p>

<p>
Consider 
the message <tt>the_quick_brown_fox</tt> encrypted with 
<i>k<sub>i</sub></i> values of 2, 3 and 1. The
encrypted string is <tt>_icuo_bfnwhoq_kxert</tt>. 
The figure below shows the decrypting right rotations for one
character in each of the three character groups.
</p>
<center><img src="./25018/file/urUGqHPI.png"></center>
<p>
Looking at all the letters in the group [a-i] we see
{<tt>i</tt>,<tt>c</tt>,<tt>b</tt>,<tt>f</tt>,<tt>h</tt>,<tt>e</tt>} 
appear at positions {2,3,7,8,11,17} within the encrypted message.
After a right rotation of <i>k<sub>1</sub></i>=2, these positions contain the
letters {<tt>h</tt>,<tt>e</tt>,<tt>i</tt>,<tt>c</tt>,<tt>b</tt>,<tt>f</tt>}.
The table below shows the intermediate strings that come from doing
all the rotations in the first group, then all rotations in the second group,
then all the rotations in the third group. Rotating letters in one group will
not change any letters in any of the other groups. 

</p>
<table width="100%">
 <tbody><tr>
   <th></th>
   <th>[a-i], <i>k<sub>1</sub></i>= 2</th>
   <th>[j-r], <i>k<sub>2</sub></i>= 3</th>

   <th>[s-z] and _, <i>k<sub>3</sub></i>= 1</th>
 </tr>

 <tr>
   <td>Encrypted:</td>
   <td><tt>_icuo_bfnwhoq_kxert</tt></td>

   <td><tt>_heuo_icnwboq_kxfrt</tt></td>
   <td><tt>_heuq_ickwbro_nxfot</tt></td>
</tr>
<tr>
   <td>Decrypted:</td>
   <td><tt>_heuo_icnwboq_kxfrt</tt></td>
   <td><tt>_heuq_ickwbro_nxfot</tt></td>

   <td><tt>the_quick_brown_fox</tt></td>
</tr>
<tr>
   <td>Changes:</td>
   <td><pre><tt> ^^   ^^  ^     ^  </tt></pre></td>
   <td><pre><tt>    ^   ^  ^^ ^  ^  </tt></pre></td>
   <td><pre><tt>^  ^ ^   ^   ^ ^  ^  </tt></pre></td>

</tr>
</tbody></table>

<p>
All input strings contain only lowercase letters and underscores(_).
Each string
will be at most 80 characters long. The <i>k<sub>i</sub></i> are all positive 
integers in the range 1-100.
</p>

<p>
Input consists of information for one or more encrypted messages.
Each problem begins with
one line containing <i>k<sub>1</sub></i>, <i>k<sub>2</sub></i>, and

<i>k<sub>3</sub></i>
followed by a line
containing the encrypted message.
The end of the input is signalled by a line with all key values of 0.
</p>

<p>For each encrypted message, the output is a single line containing
the decrypted string.
</p>

<pre><b>Input:</b>
2 3 1
_icuo_bfnwhoq_kxert
1 1 1
bcalmkyzx
3 7 4
wcb_mxfep_dorul_eov_qtkrhe_ozany_dgtoh_u_eji
2 4 3
cjvdksaltbmu
0 0 0
</pre>

<pre><b>Output:</b>
the_quick_brown_fox
abcklmxyz
the_quick_brown_fox_jumped_over_the_lazy_dog
ajsbktcludmv
</pre>