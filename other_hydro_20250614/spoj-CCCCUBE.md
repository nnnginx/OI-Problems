<p>Imagine a cube formed from solid interlocking pieces of various shapes. If the pieces are sufficiently intertwined, the only way to separate them would be to cut some of them. We can ask the question, "is the cube stable?" That is, is it physically impossible to separate the cube into 2 or more fragments without deforming and cutting any individual piece?</p>
<p>Your program must answer this question for a variety of such cubes. The pieces that make up a cube will be specified as follows: divide the cube into a grid of <em>n</em>*<em>n</em>*<em>n</em> miniature cubes, each labelled by a capital letter. Two adjacent (face-sharing) are joined together if and only if they are labelled by the same letter. For instance, the first example cube given consists of 3 solid pieces.</p>
<h3>Input</h3>
<p>Your program will be given the specification of up to 10 different cubes. The first two lines of each specification will consist of the size of that cube, <em>n</em> (1 �� n �� 10), and a blank line. There will be no spaces in the input. The input will be terminated by a number 0 on a line by itself.</p>
<h3>Output</h3>
<p>For each cube given, in the order specified, print "Yes" if that cube is stable, and "No" if it is not.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2

AB
AB

BB
BA

3

AAA
BBB
AAA

AAA
ABA
AAA

ABA
ABA
ABA

0

<strong>Output:</strong>
No
Yes

</pre>

<!--?echo("LOL");?-->