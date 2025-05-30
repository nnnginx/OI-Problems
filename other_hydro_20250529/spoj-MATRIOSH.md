<p>Vladimir worked for years making matrioshkas, those nesting dolls that certainly represent truly Russian craft. A matrioshka is a doll that may be opened in two halves, so that one finds another doll inside. Then this doll may be opened to find another one inside it. This can be repeated several times, till a final doll -that cannot be opened- is reached.

</p><p><br>Recently, Vladimir realized that the idea of nesting dolls might be generalized to nesting toys. Indeed, he has designed toys that contain toys but in a more general sense. One of these toys may be opened in two halves and it may have more than one toy inside it. That is the new feature that Vladimir wants to introduce in his new line of toys.

</p><p><br>Vladimir has developed a notation to describe how nesting toys should be constructed. A toy is represented with a positive integer, according to its size. More precisely: if when opening the toy represented by m we find the toys represented by n1, n2, . . ., nr, it must be true that n1 +n2 +. . .+nr &lt; m. And if this is the case, we say that toy m contains directly the toys n1, n2, . . ., nr . It should be clear that toys that may be contained in any of the toys n1, n2, . . ., nr are not considered as directly contained in the toy m.


</p><p><br>A generalized matrioshka is denoted with a non-empty sequence of non zero integers of the form:
a1 a2 . . . aN such that toy k is represented in the sequence with two integers −k and k, with the negative
one occurring in the sequence first that the positive one.

</p><p><br>For example, the sequence


</p><p><br></p><center>−9  −7  −2  2  −3  −2  −1  1  2  3  7  9</center>


<p><br>represents a generalized matrioshka conformed by six toys, namely, 1, 2 (twice), 3, 7 and 9.
<br>Note that toy 7 contains directly toys 2 and 3. Note that the first copy of toy 2 occurs left from the second one and that the second copy contains directly a toy 1. It would be wrong to understand that the first −2 and the last 2 should be paired.

</p><p><br>On the other hand, the following sequences do not describe generalized matrioshkas:

</p><p><br></p><center>−9  −7  −2  2  −3  −1  −2  2  1  3  7  9</center>

<p><br>because toy 2 is bigger than toy 1 and cannot be allocated inside it.

</p><p><br></p><center>−9  −7  −2  2  −3  −2  −1  1  2  3  7  −2  2  9</center>

<p><br>because 7 and 2 may not be allocated together inside 9.

</p><p><br>
</p><h3>Input</h3>
<p>The input file contains several test cases, each one of them in a separate line. Each test case is a sequence of non zero integers, each one with an absolute value less than 10^7.

</p><p><br>
</p><h3>Output</h3>
<p>Output texts for each input case are presented in the same order that input is read. For each test case the answer must be a line of the form

</p><p><br>:-) Matrioshka!
</p><p><br>if the design describes a generalized matrioshka. In other case, the answer should be of the form
</p><p><br>:-( Try again.

<br>
</p><h3>Example</h3>

<pre><b>Input:</b>
-9 -7 -2 2 -3 -2 -1 1 2 3 7 9
-9 -7 -2 2 -3 -1 -2 2 1 3 7 9
-9 -7 -2 2 -3 -1 -2 3 2 1 7 9
-100 -50 -6 6 50 100
-100 -50 -6 6 45 100
-10 -5 -2 2 5 -4 -3 3 4 10
-9 -5 -2 2 5 -4 -3 3 4 9

<b>Output:</b>
:-) Matrioshka!
:-( Try again.
:-( Try again.
:-) Matrioshka!
:-( Try again.
:-) Matrioshka!
:-( Try again.
</pre>