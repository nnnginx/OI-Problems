<p>One of the many problems in computer-generated graphics is realistically modeling the "orderly randomness" of things like mountain ranges and city skylines. A new student intern at a graphics company had an idea - use fluctuations in number representations to model height. In this problem you will compute several such number representations and show the "skylines" they produce.

</p><p>Let <b>n</b> be any positive integer, and let <b>b</b> be an integer greater than or equal to 2. The <i>complete base - <b>b</b> expansion of <b>n</b></i> is obtained as follows. First write the usual base - <b>b</b> expansion of <b>n</b>, which is just a sum of powers of <b>b</b>, each multiplied by a coefficient between 1 and <b>b</b> - 1, omitting terms with zero coefficients. For example, if <b>n</b> = 20000 and <b>b</b> = 3, the base - 3 expansion of 20000 is given by

</p><p>20000 = 3<sup>9</sup> + 3<sup>5</sup> + 2��3<sup>3</sup> + 2��3<sup>2</sup> + 2

</p><p>To obtain the complete base - <b>b</b> expansion, we apply the same procedure to the exponents until all numbers are represented in base <b>b</b>. For <b>n</b> = 20000 and <b>b</b> = 3 we would have

</p><p>20000 = 3<sup>3<sup>2</sup></sup> + 3<sup>3 + 2</sup> + 2��3<sup>3</sup> + 2��3<sup>2</sup> + 2

</p><p>As another example, consider <b>n</b> = 16647 and <b>b</b> = 2. The resulting expansion is

</p><p>16647 = 2<sup>2<sup>2 + 1</sup> + 2<sup>2</sup> + 2</sup> + 2<sup>2<sup>2 + 1</sup></sup> + 2<sup>2</sup> + 2 + 1

</p><p>The rising and falling heights of the numbers form the number's "skyline".

</p><p>For each pair of integers <b>n</b> and <b>b</b> in the input, display the complete base - <b>b</b> representation of <b>n</b>. Your display should use multiple output lines for different exponent heights. The display must begin with <i><b>n</b> = </i>, followed by the expansion. Answers should use an asterisk as the multiplication symbol between coefficients and powers of <b>b</b>. Zero terms must not be printed, and unnecessary coefficients and exponents must not be shown (for example, display 1 instead of b<sup>0</sup>, b<sup>2</sup> instead of 1*b<sup>2</sup> and b instead of b<sup>1</sup>). To assist in accurately viewing the skyline of the number, the display must show one character (either a digit, +, or *) per column of the multi-line display; there must be no unnecessary spaces. The correct format is illustrated in the sample output shown below.

</p><p>Answers must be displayed using no more than 80 columns. Expansions requiring more than 80 columns must be split between terms, into two or more sets of display lines to show the remaining portion of the expansion. The second and following parts of the answer must begin in the same column as the first part of the answer and should contain the same number of (possibly blank) lines. The split may only occur between terms of the number itself (the bottom line), not between terms in an exponent. See the sample output for an example. Note that each set of display lines starts with a blank line.</p>

<h3>Input</h3>

<p>Input is a sequence of pairs of integers, <b>n</b> and <b>b</b>, followed by a pair of zeroes. Each value for <b>n</b> will be positive, and each value for <b>b</b> will be greater than or equal to 2. All values will fit into 64 bits unsigned integers (the maximum is therefore 18446744073709551615).</p>

<h3>Output</h3>

<p>For each input pair print the complete base - <b>b</b> expansion of <b>n</b> as described above. Print a line containing</p>
<pre><b>n</b> in complete base <b>b</b>:
</pre>
<p>preceding each expansion. Separate the output for consecutive pairs by a line of exactly 80 hyphens. All coefficients, bases, and exponents are to be displayed as standard base 10 integers.</p>

<h3>Example</h3>
<pre><b>Input:</b>
20000 3
16647 2
1000 12
85026244 3
0 0

<b>Output:</b>
20000 in complete base 3:

          2
         3   3+2    3    2
20000 = 3  +3   +2*3 +2*3 +2
--------------------------------------------------------------------------------
16647 in complete base 2:

          2+1  2     2+1
         2   +2 +2  2     2
16647 = 2         +2    +2 +2+1
--------------------------------------------------------------------------------
1000 in complete base 12:

           2
1000 = 6*12 +11*12+4
--------------------------------------------------------------------------------
85026244 in complete base 3:

             2           2         2         2         2       2       2
            3 +2*3+1    3 +2*3    3 +3+2    3 +3+1    3 +2    3 +1    3
85026244 = 3        +2*3      +2*3      +2*3      +2*3    +2*3    +2*3


               2*3+2  2*3+1    3
           +2*3     +3     +2*3 +3+1
</pre>
<h3>Note</h3>
<p>The number of test cases will be no more than 100. The judge of this problem compares your output and the expected output, an extra whitespace will cause Wrong Answer.</p><p>
</p>