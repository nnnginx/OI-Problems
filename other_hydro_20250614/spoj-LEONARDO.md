<p>
<img src="./23164/file/9DYIeGQ3.png">
</p>
<p>
！ I just bought Leonardo's secret notebook!<br>
Rare object collector Stan Ucker was really agitated but
his friend, special investigator Sarah Keptic was unimpressed.<br>
！ How do you know it is genuine?<br>
！ Oh, it must be, at that price. And it is written in the
  da Vinci code.<br>
Sarah browsed a few of the pages. It was obvious
to her that the code was a substitution cipher, where each
letter of the alphabet had been substituted by another letter.<br>

！ Leonardo would have written the plain-text and left it to his
    assistant to encrypt, she said. And he must have supplied the
    substitution alphabet to be used. If we are lucky, we can find
    it on the back cover!<br>
She turned up the last page and, lo and behold, there was a single
line of all 26 letters of the alphabet:<br>
</p><blockquote>
                QWERTYUIOPASDFGHJKLZXCVBNM
</blockquote>
<p>
！ This may be Leonardo's instructions meaning that each A in the
  plain-text was to be replaced by Q, each B with W, etcetera. Let us see...<br>
To their disappointment, they soon saw that this could not be the
substitution that was used in the book. Suddenly, Stan brightened.<br>
！ Maybe Leonardo really wrote the substitution alphabet on the
last page, and by mistake his assistant coded that line as he had
coded the rest of the book. So the line we have here is the result
of applying some permutation TWICE to the ordinary alphabet!<br>

Sarah took out her laptop computer and coded fiercely for a few
minutes. Then she turned to Stan with a sympathetic expression.<br>
！ No, that couldn't be it. I am afraid that you have been duped
  again, my friend. In all probability, the book is a fake.<br>
Write a program that takes a permutation of the English alphabet as
input and decides if it may be the result of performing some
permutation twice.
</p>
<h3>Input</h3>
<p>
The input begins with a positive number on a line of its own telling
the number of test cases (at most 500).  Then for each test case there
is one line containing a permutation of the 26 capital letters of the
English alphabet.
</p>
<h3>Output</h3>
<p>
For each test case, output one line containing <tt>Yes</tt> if the
given permutation can result from applying some permutation twice on
the original alphabet string ABC...XYZ, otherwise output

<tt>No</tt>.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
2
QWERTYUIOPASDFGHJKLZXCVBNM
ABCDEFGHIJKLMNOPQRSTUVWXYZ

<b>Output:</b>
No
Yes
</pre>