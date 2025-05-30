<p>Little Johnny is playing with his small magical stamp, trying to draw a bunny on a piece of paper that is a
square k by k divided into unit squares with side 1. Johnny��s stamp is a square with side 3 and consists of
smaller squares with side 1. Exactly two of these squares are protuberant. Moreover, both protuberant squares
are in the same row or in the same column. If Johnny wants to draw pictures using this stamp, he presses it
to the piece of paper in such a way that its protuberant squares exactly match some squares of the piece of
paper. If some protuberant square touches the piece of paper, the touched square on the piece of paper changes
its colour �� from black to white or from white to black. The small stamp may lay partially outside the piece
of paper, but the protuberant squares always have to lay inside. The stamp can be shifted in any way, but it
cannot be rotated.</p><p>
In the beginning the piece of paper is whole white. The bunny consists of some number of squares that
are black (all the remaining ones have to be white). Johnny tried to draw the bunny with his small stamp for
quite a long time, but he did not succeed (this does not necessarily mean that the bunny cannot be drawn,
but only that it is very difficult to draw pictures on such a large piece of paper using such a small stamp!). So
he asked his older brother, big John, for help.</p><p>
Big John can help little Johnny by giving him his big magical stamp. The big stamp has size s by s and
has an arbitrary number of protuberant squares (these squares do not necessarily need to be located in the
same row or column). This stamp works just like the small stamp, but enforces one additional constraint �� it
can only be pressed at the piece of paper if it lies totally inside the piece of paper.</p><p>
Before big John gives little Johnny his big stamp, he would like to make sure that the stamps used together
are sufficient to draw the bunny. He asked you for help in determining that.</p>
<h3>Input</h3>
<p>The first line of the standard input contains one integer t (1 �� t �� 10) denoting the number of test cases.</p><p>
A description of a single test case starts with a line with two integers s and k (1 �� s �� k �� 1000, 1 �� s �� 200)
separated by a single space. They denote the size of big John��s stamp and the size of the piece of paper.</p><p>
The following three lines contain a description of the little Johnny��s stamp. Each of these lines contains three
characters 0 or 1. Such a description shows how does a white piece of paper look like after pressing the small
stamp: 0 represents a white square, and 1 �� a black square. Exactly two characters in these three lines are
ones and are both located either in the same row or in the same column. Please note that such description
does not illustrate the design of the stamp itself �� the stamp is symmetric to the figure drawn by it on the
piece of paper.</p><p>
The following s lines contain a description of the big John��s stamp in a similar format; this description
may, however, contain an arbitrary number of ones.
The following k lines describe the bunny, in the same format as the one used in the descriptions of stamps.
A one represents a black square, whereas a zero �� a white square.</p>

<h3>Output</h3>
<p>For each test case write out to the standard output a single line with a word TAK (��yes�� in Polish) or NIE (��no��
in Polish), depending on whether the bunny from the test case can be drawn using the stamps from the test
case (together).</p>

<h3>Example</h3>
<p>For the input data:</p>
<pre>2
3 8
010
000
010
000
010
011
01100000
00100000
00010000
00001100
00011110
10111100
01111100
01111110
5 10
001
001
000
00000
10100
00001
00001
00100
0011110000
0000111000
0010011100
0111001110
1110000000
1101001000
1000001100
0110110110
0001001000
0000110000
</pre>
<p>the correct result is:</p>
<pre>NIE
TAK
</pre>
<p>Remark: In the test data, the pictures that little Johnny is trying to draw do not need to resemble a ��real��
bunny.</p>