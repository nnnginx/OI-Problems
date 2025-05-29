<p>Thomas, a computer  scientist that works with DNA  sequences, needs to compute  longest  common  subsequences  of  given  pairs  of  strings. Consider   an    alphabet   ¦²    of   letters   and    a   word <em>w</em>=<em>a</em><sub>1</sub><em>a</em><sub>2</sub> ¡­<em>a</em><sub><em>r</em></sub>, where  <em>a</em><sub><em>i</em></sub> ¡Ê ¦², for  <em>i</em> = 1, 2,  ¡­,<em>r</em>.      A     <em>subsequence</em> of     <em>w</em> is     a     word <em>x</em>=<em>a</em><sub><em>i</em><sub>1</sub></sub><em>a</em><sub><em>i</em><sub>2</sub></sub> ¡­<em>a</em><sub><em>i</em><sub><em>s</em></sub></sub> such that 1  ¡Ü <em>i</em><sub>1</sub> &lt;  <em>i</em><sub>2</sub> &lt;   ¡­ &lt; <em>i</em><sub><em>s</em></sub> ¡Ü <em>r</em>.    Subsequence  <em>x</em> is  a  <em>segment</em> of  <em>w</em> if <em>i</em><sub><em>j</em>+1</sub>=<em>i</em><sub><em>j</em></sub> + 1, for  <em>j</em> = 1,2, ¡­,<em>s</em> -1.   For example  the word <tt>ove</tt> is a segment  of the  word <tt>lovely</tt>,  whereas the word  <tt>loly</tt> is  a subsequence  of <tt>lovely</tt>,  but  not a segment.</p>
<p>A word is a <em>common subsequence</em> of two words <em>w</em><sub>1</sub> and <em>w</em><sub>2</sub> if it is a subsequence of each  of the two words.  A <em>longest common   subsequence</em> of <em>w</em><sub>1</sub> and <em>w</em><sub>2</sub> is a common subsequence of <em>w</em><sub>1</sub> and <em>w</em><sub>2</sub> having  the largest possible length.  For  example, consider the words  <em>w</em><sub>1</sub>=<tt>lovxxelyxxxxx</tt> and <em>w</em><sub>2</sub>=<tt>xxxxxxxlovely</tt>. The words <em>w</em><sub>3</sub>=<tt>lovely</tt> and <em>w</em><sub>4</sub>=<tt>xxxxxxx</tt>, the latter of  length 7, are  both common  subsequences of  <em>w</em><sub>1</sub> and  <em>w</em><sub>2</sub>.  In fact, <em>w</em><sub>4</sub> is their longest common subsequence. Notice that the empty word, of  length zero,  is always a  common subsequence,  although not necessarily the longest.</p>
<p>In the case of Thomas,  there is an extra requirement: the subsequence must be  formed from  common segments having  length <em>K</em> or  more. For example,   if   Thomas  decides   that   <em>K</em>=3,   then  he   considers <tt>lovely</tt> to   be   an   acceptable  common   subsequence   of <tt>lovxxelyxxxxx</tt> and     <tt>xxxxxxxlovely</tt>,     whereas <tt>xxxxxxx</tt>, which has length 7 and is also a common subsequence, is not acceptable. Can you help Thomas?</p>
<h3>Input</h3>
<p>The input contains  several test cases. The first line  of a test case contains an integer <em>K</em> representing the minimum length of common segments, where 1   ¡Ü <em>K</em> ¡Ü 100.   The next  two lines  contain each  a  string on lowercase letters from the regular  alphabet of 26 letters. The length <em>l</em> of each  string satisfies  the  inequality 1   ¡Ü <em>l</em> ¡Ü 10<sup>3</sup>.  There are no spaces on any  line in the input.  The end of the input is indicated by a line containing a zero.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each  test case  in the  input, your program  must print  a single line,  containing the  length  of the  longest  subsequence formed  by consecutive segments of length at  least <em>K</em> from both strings.  If no such  common subsequence  of  length greater  than  zero exists,  then <tt>0</tt> must be printed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
lovxxelyxxxxx
xxxxxxxlovely
1
lovxxelyxxxxx
xxxxxxxlovely
3
lovxxxelxyxxxx
xxxlovelyxxxxxxx
4
lovxxxelyxxx
xxxxxxlovely
0


<strong>Output:</strong>
6
7
10
0

</pre>