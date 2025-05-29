<p>As the owner of a computer forensics company, you have just been given
     the following note by a new client:<br>
           </p>

<table cellpadding="2" cellspacing="2" border="1" style="text-align: left; width: 800px; margin-left: auto; margin-right: auto;">
           <tbody>
             <tr>
               <td valign="top">

      <p>I, Albert Charles Montgomery, have just discovered the most amazing
    cypher for encrypting messages. Let me tell you about it.&nbsp;<br>
           </p>



      <p>To begin, you will need to decide on a set of symbols, call it <span style="font-style: italic;">S</span>,   perhaps with the letters <span style="font-family: monospace;">RATE</span>. The size of this set must be
a  power of 2 and the order of the symbols in <span style="font-style: italic;">S</span> is important.   You must note that
      <span style="font-family: monospace;">R</span> is at position 0, <span style="font-family: monospace;">A</span> at 1, <span style="font-family: monospace;">T</span> at 2, and <span style="font-family: monospace;">E</span> at 3. You will   also need one permutation
      <span style="font-style: italic;">P</span> of all those symbols, say
      <span style="font-family: monospace;">TEAR</span>. Finally you will
 need an integer, call it <span style="font-style: italic;">x</span>. Together,
 these make up the key. Given a key,  you are now ready to convert a plaintext
 message <span style="font-style: italic;">M</span> of length       <span style="font-style: italic;">n</span> (<span style="font-style: italic;">M</span>[0],
      <span style="font-style: italic;">M</span>[1]... <span style="font-style: italic;">M</span>[<span style="font-style: italic;">n</span>-1]),
 that has some but not necessarily all of the symbols  in <span style="font-style: italic;">S</span>, into  a cyphertext string <span style="font-style: italic;">C</span>, also of length <span style="font-style: italic;">n</span> (<span style="font-style: italic;">C</span>[0],
       <span style="font-style: italic;">C</span>[1],...<span style="font-style: italic;">C</span>[<span style="font-style: italic;">n</span>-1]),
  that has  some but not necessarily all of the symbols in <span style="font-style: italic;">S</span>. <br>

           </p>

      <p>The encrypting algorithm computes <span style="font-style: italic;">C</span> as follows:</p>

      <ol>
         <li>Calculate an integer <span style="font-style: italic;">d</span> as the remainder after dividing the
 integer part of (<span style="font-style: italic;">n</span><sup>1.5</sup>

 + <span style="font-style: italic;">x</span>) by <span style="font-style: italic;">n</span>. This can be expressed more succinctly
 as <span style="font-style: italic;">d</span> = (int)(<span style="font-style: italic;">n</span><sup>1.5</sup> + <span style="font-style: italic;">x</span>) % <span style="font-style: italic;">n</span>, where "%" is the remainder operator.</li>

         <li>   Set <span style="font-style: italic;">C</span>[<span style="font-style: italic;">d</span>] to be the symbol in <span style="font-style: italic;">S</span> whose position is the  same   as the
 position of <span style="font-style: italic;">M</span>[<span style="font-style: italic;">d</span>] in <span style="font-style: italic;">P</span>.<br>

         </li>
         <li>    For each <span style="font-style: italic;">j</span> �� <span style="font-style: italic;">d</span> in 0..<span style="font-style: italic;">n</span>-1,
              set <span style="font-style: italic;">C</span>[<span style="font-style: italic;">j</span>] to be the symbol in <span style="font-style: italic;">S</span> whose position is the  value   obtained
 by xor-ing the position of <span style="font-style: italic;">M</span>[<span style="font-style: italic;">j</span>] in <span style="font-style: italic;">P</span> with the position  of <span style="font-style: italic;">M</span>[(<span style="font-style: italic;">j</span>+1)
% <span style="font-style: italic;">n</span>]   in <span style="font-style: italic;">S</span>. Note that the bitwise xor operator
 is "^" in C, C++, and Java. </li>

      </ol>
<p>For example, consider this scenario where <span style="font-style: italic;">S</span>=<span style="font-family: monospace;">RATE</span>, <span style="font-style: italic;">P</span>=<span style="font-family: monospace;">TEAR</span>, <span style="font-style: italic;">x</span>=102,  <span style="font-style: italic;">M</span>=<span style="font-family: monospace;">TEETER</span>, and <span style="font-style: italic;">n</span>=6. To compute <span style="font-style: italic;">d</span>, first calculate 6<sup>1.5</sup> + 102
= 116.696938, then take the remainder after dividing by 6. So  <span style="font-style: italic;">d</span> = 116 % 6 = 2. The following table
 shows the steps in filling in the cyphertext  <span style="font-style: italic;">C</span>. Note  that the order of the steps is
not important.</p>

      <table cellpadding="2" cellspacing="2" border="1" style="text-align: left; width: 90%; margin-left: 40px;">
            <tbody>
              <tr>
                <td valign="top"><br>
                </td>
                <td valign="top">0<br>
                </td>
                <td valign="top">1<br>

                </td>
                <td valign="top">2<br>
                </td>
                <td valign="top">3<br>
                </td>
                <td valign="top">4<br>
                </td>

                <td valign="top">5<br>
                </td>
                <td valign="top"><br>
                </td>
              </tr>
              <tr>
                   <td valign="top"><span style="font-style: italic;">S</span>
 =<br>

                   </td>
                   <td valign="top" style="font-family: monospace;">R<br>
                   </td>
                   <td valign="top" style="font-family: monospace;">A<br>
                   </td>
                   <td valign="top" style="font-family: monospace;">T<br>
                   </td>

                   <td valign="top" style="font-family: monospace;">E<br>
                   </td>
                   <td valign="top" style="font-family: monospace;"><br>
                   </td>
                   <td valign="top" style="font-family: monospace;"><br>
                   </td>
                   <td valign="top"><br>
                   </td>

                 </tr>
                 <tr>
                   <td valign="top"><span style="font-style: italic;">P</span>
 = <br>
                   </td>
                   <td valign="top" style="font-family: monospace;">T<br>
                   </td>

                   <td valign="top" style="font-family: monospace;">E<br>
                   </td>
                   <td valign="top" style="font-family: monospace;">A<br>
                   </td>
                   <td valign="top" style="font-family: monospace;">R<br>
                   </td>
                   <td valign="top" style="font-family: monospace;"><br>

                   </td>
                   <td valign="top" style="font-family: monospace;"><br>
                   </td>
                   <td valign="top"><br>
                   </td>
                 </tr>
                 <tr>
                <td valign="top"><span style="font-style: italic;">M</span>

 =<br>
                </td>
                <td valign="top" style="font-family: monospace;">T<br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>

                </td>
                <td valign="top" style="font-family: monospace;">T<br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">R<br>
                </td>

                <td valign="top"><br>
                </td>
              </tr>
              <tr>
                   <td valign="top"><br>
                   </td>
                   <td valign="top"><br>
                   </td>
                   <td valign="top"><br>

                   </td>
                   <td valign="top"><br>
                   </td>
                   <td valign="top"><br>
                   </td>
                   <td valign="top"><br>
                   </td>
                   <td valign="top"><br>
                   </td>

                   <td valign="top"><span style="font-style: italic;"></span><br>
                 </td>
                 </tr>
                 <tr>
                <td valign="top"><span style="font-style: italic;">C</span>
 = <br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>

                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>

                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top"><span style="font-style: italic;"></span><span style="font-style: italic;">M</span>[0] is <span style="font-family: monospace;">T</span>, <span style="font-family: monospace;">T</span> is at <span style="font-style: italic;">P</span>[0]. <span style="font-style: italic;">M</span>[1] is <span style="font-family: monospace;">E</span>, <span style="font-family: monospace;">E</span> is at <span style="font-style: italic;">S</span>[3]. <span style="font-style: italic;">C</span>[0] = <span style="font-style: italic;">S</span>[0 xor 3] = <span style="font-style: italic;">S</span>[3]<br>

                </td>
              </tr>
              <tr>
                <td valign="top"><br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">T<br>

                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>

                <td valign="top"><span style="font-style: italic;">M</span>[1]
 is <span style="font-family: monospace;">E</span>, <span style="font-family: monospace;">E</span> is at <span style="font-style: italic;">P</span>[1]. <span style="font-style: italic;">M</span>[2] is <span style="font-family: monospace;">E</span>, <span style="font-family: monospace;">E</span> is at <span style="font-style: italic;">S</span>[3].    <span style="font-style: italic;">C</span>[1] = <span style="font-style: italic;">S</span>[1 xor 3] = <span style="font-style: italic;">S</span>[2]<br>

                </td>
              </tr>
              <tr>
                <td valign="top"><br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">T<br>

                </td>
                <td valign="top" style="font-family: monospace;">A<br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>

                </td>
                <td valign="top"><span style="font-style: italic;"></span><span style="font-style: italic;">2 is d. M</span>[2] is <span style="font-family: monospace;">E</span>, <span style="font-family: monospace;">E</span> is at <span style="font-style: italic;">P</span>[1], so <span style="font-style: italic;">C</span>[2] =&nbsp; <span style="font-style: italic;">S</span>[1]<br>

                </td>
              </tr>
              <tr>
                <td valign="top"><br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">T<br>

                </td>
                <td valign="top" style="font-family: monospace;">A<br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top" style="font-family: monospace;"><br>

                </td>
                <td valign="top"><span style="font-style: italic;">M</span>[3]
 is <span style="font-family: monospace;">T</span>, <span style="font-family: monospace;">T</span> is at <span style="font-style: italic;">P</span>[0]. <span style="font-style: italic;">M</span>[4] is <span style="font-family: monospace;">E</span>, <span style="font-family: monospace;">E</span> is at <span style="font-style: italic;">S</span>[3]. <span style="font-style: italic;">C</span>[3] = <span style="font-style: italic;">S</span>[0 xor 3] = <span style="font-style: italic;">S</span>[3]<br>

                </td>
              </tr>
              <tr>
                <td valign="top"><br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">T<br>

                </td>
                <td valign="top" style="font-family: monospace;">A<br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">A<br>
                </td>

                <td valign="top" style="font-family: monospace;"><br>
                </td>
                <td valign="top"><span style="font-style: italic;">M</span>[4]
 is <span style="font-family: monospace;">E</span>, <span style="font-family: monospace;">E</span> is at <span style="font-style: italic;">P</span>[1]. <span style="font-style: italic;">M</span>[5] is <span style="font-family: monospace;">R</span>, <span style="font-family: monospace;">R</span> is at <span style="font-style: italic;">S</span>[0].    <span style="font-style: italic;">C</span>[4] = <span style="font-style: italic;">S</span><span style="font-style: italic;"></span>[1
 xor 0] = <span style="font-style: italic;">S</span>[1]<br>

                </td>
              </tr>
              <tr>
                <td valign="top"><br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">T<br>

                </td>
                <td valign="top" style="font-family: monospace;">A<br>
                </td>
                <td valign="top" style="font-family: monospace;">E<br>
                </td>
                <td valign="top" style="font-family: monospace;">A<br>
                </td>

                <td valign="top" style="font-family: monospace;">A<br>
                </td>
                <td valign="top"><span style="font-style: italic;">M</span>[5]
 is <span style="font-family: monospace;">R</span>, <span style="font-family: monospace;">R</span> is at <span style="font-style: italic;">P</span>[3]. <span style="font-style: italic;">M</span>[0] is <span style="font-family: monospace;">T</span>, <span style="font-family: monospace;">T</span> is at <span style="font-style: italic;">S</span>[2].    <span style="font-style: italic;">C</span>[5] = <span style="font-style: italic;">S</span>[3 xor 2] = <span style="font-style: italic;">S</span>[1]<br>

                </td>
              </tr>


        </tbody>

      </table>

      <div style="margin-left: 40px;"> </div>
          <br>

           I have included additional examples of encrypted messages at the
 end   of  this note for you to experiment with. However, first, I need to
 tell  you about the decryption algorithm.</td>
             </tr>

  </tbody>
</table>

<p>Unfortunately, the next page of the note, with the decrypting algorithm,
     is completely unreadable because it is covered with huge, overlapping,
  messy   ink blots. Given your considerable skill in unravelling puzzles,
 your task   is to write the decoder based on your knowledge of the encoding
 algorithm.</p>

<h3>Input</h3>
<p> The input for the decoder
   consists of one or more sets of {key, encrypted   message} pairs. The
key    is on 3 separate lines. The first line contains the  single integer
<span style="font-style: italic;">x</span>, 0 &lt; <span style="font-style: italic;">x</span> &lt; 10,000; the second line contains
 the string <span style="font-style: italic;">S</span>; and the third line
 contains the string <span style="font-style: italic;">P</span>, which
   will be a permutation of <i>S</i>.  The length of
 <span style="font-style: italic;">S</span> (and therefore <span style="font-style: italic;">P</span>)
   will always be one of the following powers of two: 2, 4, 8, 16, or
   32.  Following the key is a line containing
  the encrypted message string <span style="font-style: italic;">C</span>, which
 will contain at least one and at most sixty characters.
 The strings <span style="font-style: italic;">S</span>, <span style="font-style: italic;">P</span>, and <span style="font-style: italic;">C</span> will not contain whitespace, but may
   contain printable characters other than letters and digits.
 The end of the input is a line  which contains
 the single integer 0. </p>


<h3>Output</h3>
<p>For each input set print
  the decrypted string on a single line, as shown    in the  sample output.
  </p>


<h3>Example</h3>

<pre><b>Input:</b>
102
RATE
TEAR
ETAEAA
32
ABCDEFGHIJKLMNOPQRSTUVWXYZ._!?,;
;ABCDEFGHIJKLMNOPQRSTUVWXYZ._!?,
MOMCUKZ,ZPD
1956
ACEHINT_
ACTN_IHE
CIANCTNAAIECIA_TAI
0

<b>Output:</b>
TEETER
HELLO_WORLD
THE_CAT_IN_THE_HAT

</pre>