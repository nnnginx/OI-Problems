<p>Prof. Hachioji has devised a new numeral system of integral numbers with four lowercase letters "m", "c", "x", "i" and with eight digits "2", "3", "4", "5", "6", "7", "8", "9". He doesn't use digit "0" nor digit "1" in this system.

</p><p></p><p>
The letters "m", "c", "x" and "i" correspond to 1000, 100, 10 and 1, respectively, and the digits "2", ...,"9" correspond to 2, ..., 9, respectively. This system has nothing to do with the Roman numeral system.

</p><p></p><p>
For example, character strings

</p><p></p><p>
    "5m2c3x4i", "m2c4i" and "5m2c3x" 

</p><p></p><p>
correspond to the integral numbers 5234 (=5*1000+2*100+3*10+4*1), 1204 (=1000+2*100+4*1), and 5230 (=5*1000+2*100+3*10), respectively. The parts of strings in the above example, "5m", "2c", "3x" and "4i" represent 5000 (=5*1000), 200 (=2*100), 30 (=3*10) and 4 (=4*1), respectively.

</p><p></p><p>
Each of the letters "m", "c", "x" and "i" may be prefixed by one of the digits "2", "3", ..., "9". In that case, the prefix digit and the letter are regarded as a pair. A pair that consists of a prefix digit and a letter corresponds to an integer that is equal to the original value of the letter multiplied by the value of the prefix digit.

</p><p></p><p>
For each letter "m", "c", "x" and "i", the number of its occurrence in a string is at most one. When it has a prefix digit, it should appear together with the prefix digit. The letters "m", "c", "x" and "i" must appear in this order, from left to right. Moreover, when a digit exists in a string, it should appear as the prefix digit of the following letter. Each letter may be omitted in a string, but the whole string must not be empty. A string made in this manner is called an MCXI-string.

</p><p></p><p>
An MCXI-string corresponds to a positive integer that is the sum of the values of the letters and those of the pairs contained in it as mentioned above. The positive integer corresponding to an MCXI-string is called its MCXI-value. Moreover, given an integer from 1 to 9999, there is a unique MCXI-string whose MCXI-value is equal to the given integer. For example, the MCXI-value of an MCXI-string "m2c4i" is 1204 that is equal to 1000 + 2*100 + 4*1. There are no MCXI-strings but "m2c4i" that correspond to 1204. Note that strings "1m2c4i", "mcc4i", "m2c0x4i", and "2cm4i" are not valid MCXI-strings. The reasons are use of "1", multiple occurrences of "c", use of "0", and the wrong order of "c" and "m", respectively.

</p><p></p><p>
Your job is to write a program for Prof. Hachioji that reads two MCXI-strings, computes the sum of their MCXI-values, and prints the MCXI-string corresponding to the result. 

</p><p>
</p><h3>Input</h3>
<p>
The input is as follows. The first line contains a positive integer n (&lt;= 500) that indicates the number of the following lines. The k+1 th line is the specification of the k th computation (k=1, ..., n).

</p><p></p><p>
    n<br>
    specification1<br>
    specification2<br>
    ...<br>
    specificationn<br>

</p><p></p><p>
Each specification is described in a line:

</p><p></p><p>
    MCXI-string1 MCXI-string2 

</p><p></p><p>
The two MCXI-strings are separated by a space.

</p><p></p><p>
You may assume that the sum of the two MCXI-values of the two MCXI-strings in each specification is less than or equal to 9999. 

</p><h3>Output</h3>
<p>For each specification, your program should print an MCXI-string in a line. Its MCXI-value should be the sum of the two MCXI-values of the MCXI-strings in the specification. No other characters should appear in the output.

</p><h3>Example</h3>

<pre><b>Input:</b>
10
xi x9i
i 9i
c2x2i 4c8x8i
m2ci 4m7c9x8i
9c9x9i i
i 9m9c9x8i
m i
i m
m9i i
9m8c7xi c2x8i

<b>Output:</b>
3x
x
6cx
5m9c9x9i
m
9m9c9x9i
mi
mi
mx
9m9c9x9i
</pre>