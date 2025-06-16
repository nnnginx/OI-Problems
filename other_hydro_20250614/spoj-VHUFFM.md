<p>
Huffman encoding is a method of developing an optimal encoding of the symbols 
in a <i>source alphabet</i> using symbols from a <i>target alphabet</i> when the frequencies
of each of the symbols in the source alphabet are known. Optimal means the 
average length of an encoded message will be minimized. In this problem you 
are to determine an encoding of the first <i>N</i> uppercase letters (the source
alphabet,  <img width="16" height="25" align="MIDDLE" alt="tex2html_wrap_inline87" src="/content/ak15:240img1.gif">  through  <img width="22" height="25" align="MIDDLE" alt="tex2html_wrap_inline89" src="/content/ak15:240img2.gif"> , with frequencies  <img width="13" height="25" align="MIDDLE" alt="tex2html_wrap_inline91" src="/content/ak15:240img3.gif">  through  <img width="20" height="25" align="MIDDLE" alt="tex2html_wrap_inline93" src="/content/ak15:240img4.gif"> ) into the
first <i>R</i> decimal digits (the target alphabet,  <img width="16" height="25" align="MIDDLE" alt="tex2html_wrap_inline97" src="/content/ak15:240img5.gif">  through  <img width="21" height="25" align="MIDDLE" alt="tex2html_wrap_inline99" src="/content/ak15:240img6.gif"> ).

</p><p>
</p><p>
Consider determining the encoding when <i>R</i>=2. Encoding proceeds in several
passes. In each pass the two source symbols with the lowest frequencies, say 
 <img width="16" height="25" align="MIDDLE" alt="tex2html_wrap_inline87" src="/content/ak15:240img1.gif">  and  <img width="16" height="25" align="MIDDLE" alt="tex2html_wrap_inline105" src="/content/ak15:240img7.gif"> , are grouped to form a new ``combination letter" whose frequency is
the sum of  <img width="13" height="25" align="MIDDLE" alt="tex2html_wrap_inline91" src="/content/ak15:240img3.gif">  and  <img width="14" height="25" align="MIDDLE" alt="tex2html_wrap_inline109" src="/content/ak15:240img8.gif"> . If there is a tie for the lowest or second lowest
frequency, the letter occurring earlier in the alphabet is selected. After 
some number of passes only two letters remain to be combined. The letters 
combined in each pass are assigned one of the symbols from the target 
alphabet.
</p><p>
</p><p>

The letter with the lower frequency is assigned the code 0, and the 
other letter is assigned the code 1. (If each letter in a combined group has 
the same frequency, then 0 is assigned to the one earliest in the alphabet. 
For the purpose of comparisons, the value of a ``combination letter" is the
value of the earliest letter in the combination.) The final code sequence for 
a source symbol is formed by concatenating the target alphabet symbols 
assigned as each combination letter using the source symbol is formed.
</p><p>
The 
target symbols are concatenated in the reverse order that they are assigned so 
that the first symbol in the final code sequence is the last target symbol 
assigned to a combination letter.
</p><p>
</p><p>
The two illustrations below demonstrate the 
process for <i>R</i>=2.
</p><p>
</p><p> <img align="BOTTOM" alt="tabular23" src="/content/ak15:240img9.gif"> </p><p>
</p><p>
When <i>R</i> is larger than 2, <i>R</i> symbols are grouped in each pass. Since each pass
effectively replaces <i>R</i> letters or combination letters by 1 combination letter,
and the last pass must combine <i>R</i> letters or combination letters, the source
alphabet must contain <i>k</i>*(<i>R</i>-1)+<i>R</i> letters, for some integer <i>k</i>.

</p><p>
Since <i>N</i>
may not be this large, an appropriate number of fictitious letters with zero
frequencies must be included. These fictitious letters are not to be included 
in the output. In making comparisons, the fictitious letters are later than 
any of the letters in the alphabet.
</p><p>
</p><p>
Now the basic process of determining the Huffman encoding is the same as for 
the <i>R</i>=2 case. In each pass, the <i>R</i> letters with the lowest frequencies are
grouped, forming a new combination letter with a frequency equal to the sum of 
the letters included in the group. The letters that were grouped are assigned 
the target alphabet symbols 0 through <i>R</i>-1. 0 is assigned to the letter in the
combination with the lowest frequency, 1 to the next lowest frequency, and so 
forth. If several of the letters in the group have the same frequency, the one 
earliest in the alphabet is assigned the smaller target symbol, and so forth.
</p><p>
</p><p>

The illustration below demonstrates the process for <i>R</i>=3.
</p><p>
</p><p> <img width="383" height="190" align="BOTTOM" alt="tabular63" src="/content/ak15:240img10.gif"> </p><p>
</p><h3>Input</h3>
<p>The input will contain one or more data sets, one per line. Each data set 
consists of an integer value for <i>R</i> (between 2 and 10), an integer value for <i>N</i>
(between 2 and 26), and the integer frequencies  <img width="13" height="25" align="MIDDLE" alt="tex2html_wrap_inline91" src="/content/ak15:240img3.gif">  through  <img width="20" height="25" align="MIDDLE" alt="tex2html_wrap_inline93" src="/content/ak15:240img4.gif"> , each of which
is between 1 and 999.

</p><p>
The end of data for the entire input is the number 0 for 
<i>R</i>; it is not considered to be a separate data set.
</p><p>

</p><h3>Output</h3>
<p>For each data set, display its number (numbering is sequential starting with 
1) and the average target symbol length (rounded to two decimal places) on one 
line. Then display the <i>N</i> letters of the source alphabet and the corresponding 
Huffman codes, one letter and code per line. 
<br>Print a blank line after each test case.
<br>
The examples below illustrate the 
required output format.</p>
<h3>Example</h3>

<pre><b>Input:</b>

2 5 5 10 20 25 40
2 5 4 2 2 1 1
3 7 20 5 8 5 12 6 9
4 6 10 23 18 25 9 12
0

<b>Output:</b>

Set 1; average length 2.10
    A: 1100
    B: 1101
    C: 111
    D: 10
    E: 0

Set 2; average length 2.20
    A: 11
    B: 00
    C: 01
    D: 100
    E: 101

Set 3; average length 1.69
    A: 1
    B: 00
    C: 20
    D: 01
    E: 22
    F: 02
    G: 21

Set 4; average length 1.32
    A: 32
    B: 1
    C: 0
    D: 2
    E: 31
    F: 33
</pre>