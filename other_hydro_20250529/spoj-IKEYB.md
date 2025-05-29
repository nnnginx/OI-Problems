<p>
Most of you have probably tried to type an&nbsp;SMS message on the keypad of
a&nbsp;cellular phone. It is sometimes very annoying to write longer messages,
because one key must be usually pressed several times to produce a&nbsp;single
letter. It is due to a&nbsp;low number of keys on the keypad. Typical phone has
twelve keys only (and maybe some other control keys that are not used for
typing). Moreover, only eight keys are used for typing 26&nbsp;letters of
an&nbsp;English alphabet. The standard assignment of letters on the keypad is
shown in the left picture:

</p><p>

</p><table align="CENTER"><tbody><tr><td>

<table bordercolor="BLACK" cellpadding="3" cellspacing="0" border="1">
<tbody><tr><td align="CENTER">1<br>&nbsp;</td>
<td align="CENTER">2<br>abc</td>
<td align="CENTER">3<br>def</td>
</tr>
<tr><td align="CENTER">4<br>ghi</td>
<td align="CENTER">5<br>jkl</td>
<td align="CENTER">6<br>mno</td>
</tr>
<tr><td align="CENTER">7<br>pqrs</td>
<td align="CENTER">8<br>tuv</td>
<td align="CENTER">9<br>wxyz</td>
</tr>
<tr><td align="CENTER">*<br>&nbsp;</td>
<td align="CENTER">0<br><em>space</em></td>
<td align="CENTER">#<br>&nbsp;</td>
</tr>
</tbody></table>

</td><td>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td><td>

<table bordercolor="BLACK" cellpadding="3" cellspacing="0" border="1">
<tbody><tr><td align="CENTER">1<br>&nbsp;</td>
<td align="CENTER">2<br>abcd</td>
<td align="CENTER">3<br>efg</td>
</tr>
<tr><td align="CENTER">4<br>hijk</td>
<td align="CENTER">5<br>lm</td>
<td align="CENTER">6<br>nopq</td>
</tr>
<tr><td align="CENTER">7<br>rs</td>
<td align="CENTER">8<br>tuv</td>
<td align="CENTER">9<br>wxyz</td>
</tr>
<tr><td align="CENTER">*<br>&nbsp;</td>
<td align="CENTER">0<br><em>space</em></td>
<td align="CENTER">#<br>&nbsp;</td>
</tr>
</tbody></table>

</td></tr>
</tbody></table>

<p>
There are 3 or 4 letters assigned to each key. If you want the first letter
of any group, you press that key once. If you want the second letter, you
have to press the key twice. For other letters, the key must be pressed three
or four times. The authors of the keyboard did not try to optimise the layout
for minimal number of keystrokes. Instead, they preferred the even
distribution of letters among the keys. Unfortunately, some letters are more
frequent than others. Some of these frequent letters are placed on the third
or even fourth place on the standard keyboard. For
example, <tt>S</tt> is a&nbsp;very common letter in an&nbsp;English alphabet, and we need
four keystrokes to type it. If the assignment of characters was like in the
right picture, the keyboard would be much more comfortable for typing average
English texts.

</p><p>
ACM have decided to put an&nbsp;optimised version of the keyboard on its new
cellular phone. Now they need a&nbsp;computer program that will find an&nbsp;optimal
layout for the given letter frequency. We need to preserve alphabetical
order of letters, because the user would be confused if the letters were
mixed. But we can assign any number of letters to a&nbsp;single key.

</p><p>
</p><h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 2000). It stands
for the number of test cases to follow. Each test case begins with a&nbsp;line
containing two integers <var>K</var>, <var>L</var> (1  &lt;= <var>K</var>  &lt;= <var>L</var>  &lt;= 90) separated by
a&nbsp;single space. <var>K</var> is the number of keys, <var>L</var> is the number of letters to be
mapped onto those keys. Then there are two lines. The first
one contains exactly <var>K</var> characters each representing a&nbsp;name of one
key. The second line contains exactly <var>L</var> characters representing names
of letters of an&nbsp;alphabet. Keys and letters are represented by digits,
letters (which are case-sensitive), or any punctuation characters (ASCII code
between 33 and 126 inclusively). No two keys have the same character, no two
letters are the same. However, the name of a&nbsp;letter can be used also as
a&nbsp;name for a&nbsp;key.

</p><p>
After those two lines, there are exactly <var>L</var> lines each containing exactly
one positive integer <var>F</var><sub>1</sub>, <var>F</var><sub>2</sub>, ... <var>F</var><sub><var>L</var></sub>. These numbers determine the
frequency of every letter, starting with the first one and continuing with
the others sequentially. The higher number means the more common letter. No
frequency will be higher than 100000.

</p><p>
</p><h3>Output</h3>

<p>
Find an&nbsp;optimal keyboard for each test case. Optimal keyboard is such that
has the lowest "price" for typing average text. The <em>price</em> is determined
as the sum of the prices of each letter. The price of a&nbsp;letter is a&nbsp;product
of the&nbsp;letter frequency (<var>F</var><sub><var>i</var></sub>) and its position on the key. The order of
letters cannot be changed, they must be grouped in the given order.

</p><p>
If there are more solutions with the same price, we will try to maximise the
number of letters assigned to the last key, then to the one before the last
one etc.

</p><p>
More formally, you are to find a&nbsp;sequence <var>P</var><sub>1</sub>, <var>P</var><sub>2</sub>, ... <var>P</var><sub><var>L</var></sub> 
representing the position of every letter on a&nbsp;particular key. The sequence
must meet following conditions:
</p><div align="left">
<ul>
<li><var>P</var><sub>1</sub> = 1
</li><li>for each <var>i</var>&gt;1, either 
<var>P</var><sub><var>i</var></sub> = <var>P</var><sub><var>i</var>-1</sub>+1 or <var>P</var><sub><var>i</var></sub> = 1
</li><li>there are at most <var>K</var> numbers <var>P</var><sub><var>i</var></sub> such that <var>P</var><sub><var>i</var></sub> = 1
</li><li>the sum of products <var>S</var><sub><var>P</var></sub> = 
Sum[i=1..l]
<var>F</var><sub><var>i</var></sub>.<var>P</var><sub><var>i</var></sub> is minimal
</li><li>for any other sequence <var>Q</var> meeting these criteria and with the same
  sum <var>S</var><sub><var>Q</var></sub> = <var>S</var><sub><var>P</var></sub>, there exists such <var>M</var>, 
1 &lt;= <var>M</var> &lt;= <var>L</var> that for any <var>J</var>,
  <var>M</var>&lt;<var>J</var> &lt;= <var>L</var>, <var>P</var><sub><var>J</var></sub> = <var>Q</var><sub><var>J</var></sub>, and <var>P</var><sub><var>M</var></sub>&gt;<var>Q</var><sub><var>M</var></sub>.
</li></ul>
</div>
<p>
The output for every test case must start with a&nbsp;single line saying
<tt>Keypad #</tt><var>I</var><tt>:</tt>, where <var>I</var> is a&nbsp;sequential order of the test case,
starting with 1. Then there must be exactly <var>K</var> lines, each representing one
letter, in the same order that was used in input. Each line must contain the
character representing the key, a&nbsp;colon, one space and a&nbsp;list of letters
assigned to that particular key. Letters are not separated from each other.

</p><p>
Print one blank line after each test case, including the last one.


</p><h3>Example</h3>
<p>Sample Input:</p>

<pre><tt>1
8 26
23456789
ABCDEFGHIJKLMNOPQRSTUVWXYZ
3371
589
1575
1614
6212
971
773
1904
2989
123
209
1588
1513
2996
3269
1080
121
2726
3083
4368
1334
518
752
427
733
871
</tt>
</pre>

<p>Sample Output:</p>

<pre><tt>Keypad #1:
2: ABCD
3: EFG
4: HIJK
5: LM
6: NOPQ
7: RS
8: TUV
9: WXYZ
</tt></pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>