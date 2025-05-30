<p align="justify">The Maya lived in Central America during the first millennium. In many regards, they consituted one of the most developed and most fascinating cultures of this epoch. Even though draught animals and the wheel were unknown to the Mayas, they excelled in the fields of weaving, architecture and pottery. But truely breath-taking were their achievements in the fields of astronomy and mathematics. Whilst Europe was trudging through the dark Middle Ages, the Maya determined the solar year to 365.242 days (modern-day measurement: 365.242198) and the lunar cycle to 29.5302 days (modern-day measurement: 29.53059). Such astonishingly precise findings were hardly possible without a powerful numeral system. In this task we will explore the Maya's numeral system.</p>
<p align="justify">Maya priests and astronomers used a numerical system to the base of 20. Unusual to their time, their system also included the concepts of digits and of the zero. Both concepts were completely unknown to the Europeans at this time. The first nineteen numbers of the vigesimal system were represented by dots and dashes according to the following table:</p>
<p align="justify"><img src="/content/ahven:table.gif"></p>
<p align="justify">The zero was written down as a symbol resembling a shell. Multi-digit numbers (i.e. the numbers bigger than 19) were written in vertical arrangement, with the highest-value digit on top. For example, the number 79 was written as</p>
<p align="justify"><img src="/content/ahven:num1.gif"></p>
<p align="justify">As can be seen, the second digit possesses a value of 20.</p>
<p align="justify">Due to an interference of the two calendar systems of the Maya, the third digit did not hold the value 400 (20x20), as would be expected, but 360. All the following digits were again treated regularly, i.e. the fourth digit counted 7200 (360x20), the fifth 144000 (7200x20), and so on.</p>
<p align="justify">Hence, the number 13495 (=1x7200+17x360+8x20+15) was written as follows:</p>
<p align="justify"><img src="/content/ahven:num2.gif"></p>
<p align="justify">Write a program to convert Maya numbers to decimal numbers!</p>

<h3>Input</h3>
<p align="justify">The input file contains a list of numbers written down in Maya fashion. Of course, dots are represented as points (.), and dashes are represented as hyphens (-). The zero digit, the shell symbol, is written as a capital letter S (S). Description of a Maya number starts with <i>n</i> - the number of the Maya digits. The following <i>n</i> lines contain one digit each. One digit is written from top to bottom using spaces as vertical separators.</p>
<p align="justify">One number will not have more than seven digits. Each two numbers are separated by a blank line. Input terminates with <i>n</i> = 0</p>

<h3>Output</h3>
<p align="justify">Your program has to output the value of the number in the input file in the nowadays more common decimal system. One number per line.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
..

5
... -
. - -
S
S
S

0
<b><tt>Sample output:</tt></b>
2
1231200
</pre>