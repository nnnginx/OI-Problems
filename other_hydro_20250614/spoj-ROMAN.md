<p>
Given the number n of test cases, convert n positive integers less than 2^32 (given one per line) from one representation to another.
For convenience, n is given in the same format as the other numbers.

</p><h3>Input</h3>
<p>
Input is given by spelling the number in english digits (all upper case letters). Thus the range of (32-bit) input values permissible extends from ZERO (or OH) through FOUR TWO NINE FOUR NINE SIX SEVEN TWO NINE FIVE.

</p><h3>Output</h3>
<p>
Output 2 lines for each test case.
Output is in the form of "extended" Roman numerals (also called "butchered" Roman numerals), with an overline (see sample for details) indicating the value below is "times 1000", and lower-case letters indicating "times 1000000". Thus, the range of (32-bit) output values possible is from through ivccxcivCMLXVIICCXCV, where there is a line above iv and CMLXVII. Note: For values whose residues modulo 1000000 are less than 4000, M is used to represent 1000; for values whose residues are 4000 or greater, I is used. Thus 3999 would read out as MMMCMXCIX while 4000 would readout as IV with an overline. Similar rules apply to the use of M and i for 1000000, and to that of m and i for 1000000000.

</p><p>
<b> WARNING: This problem has a somewhat strict source limit </b>

</p><h3>Example</h3>
<pre><b>Input:</b>
THREE
FOUR OH
ONE NINE NINE NINE NINE NINE NINE NINE NINE NINE
ONE TWO THREE ZERO FOUR FIVE

<b>Output:</b>
  
XL
       ______      
mcmxcixCMXCIXCMXCIX
___      
CXXMMMXLV
</pre>