<p><i>Little Quilt</i> is a small language introduced by Ravi Sethi in his book ¡®Programming Languages¡¯.

</p><p><br>Here, a restricted version of Little Quilt is presented. The language is defined by the following BNF grammar:

</p><p><br>
&lt; QUILT &gt; ::= A | B | turn(&lt; QUILT &gt;) | sew(&lt; QUILT &gt;,&lt; QUILT &gt;)


</p><p><br>A and B represent the two primitive quilts. Each primitive quilt corresponds to a matricial arrangement of 2 ¡Á 2 characters. turn() and sew() are operations over quilts.

</p><p><br>The instruction turn(x) turns the quilt x 90 degrees clockwise. The following table illustrates the primitive quilts as well as examples of the effect of the turn() operation:

</p><p><br>
</p><center><img src="/content/steinersp:quilt1.jpg" alt="subir imagenes" border="0"></center>

<p><br>
Accordingly, the instruction sew(x,y) sews quilt x to the left of quilt y. Both x and y must have the same height, otherwise an error will be generated. The following figure represents the result of sew(A,turn(B)):

</p><p><br>
</p><center><img src="/content/steinersp:quilt2.jpg" alt="subir imagenes" border="0"></center>

<p><br>while the sew(turn(sew(B,turn(B))),A) generates an error message.

</p><p><br>Your job is to build an interpreter of the Little Quilt language.

</p><p><br>
</p><h3>Input</h3>
<p>The input file will be a text file containing different Little Quilt expressions, each one ended by a semicolon character (;). Space and new line characters must be ignored; this means that an expression may span several lines.

</p><p><br>
</p><h3>Output</h3>
<p>The output file contains the quilts produced as a result of interpreting the input expressions.

</p><p><br>Each quilt must be preceded by a line, left aligned, with the format

</p><p><br>Quilt i:
<br>where i is the quilt number, starting at 1. If the expression interpretation generates and error, the word

</p><p><br>error
<br>must be printed.

</p><p><br>
</p><h3>Example</h3>

<pre><b>Input:</b>
sew(turn(sew(B,turn(B))),
turn(sew(turn(B),B))) ;
<br><br>
sew(turn(sew(B,turn(B))),A);
sew(turn(sew(A,turn(A))),
turn(turn(
<br>
turn(sew(A,turn(A))))))
;

<b>Output:</b>
Quilt 1:
||--
||--
--||
--||
Quilt 2:
error
Quilt 3:
\\//
+\/+
+/\+
//\\
</pre>