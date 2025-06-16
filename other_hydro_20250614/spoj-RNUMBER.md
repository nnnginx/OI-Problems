<p>A Black Box algorithm supposes that natural
number sequence 
<img width="155" height="34" align="MIDDLE" border="0" src="/content/ak15:504img1.gif" alt="$u(1), u(2), dots, u(N)$">
is sorted
in non-descending order, <img width="63" height="32" align="MIDDLE" border="0" src="/content/ak15:504img2.gif" alt="$N le M$">
and for each <i>p</i>
(
<img width="84" height="32" align="MIDDLE" border="0" src="/content/ak15:504img3.gif" alt="$1 le p le N$">)
an inequality 
<img width="111" height="34" align="MIDDLE" border="0" src="/content/ak15:504img4.gif" alt="$p le u(p) le M$">
is valid.
</p>
<p>
<br>
Making tests for this algorithm we have met with the following problem.
For setting a random sequence
<img width="52" height="34" align="MIDDLE" border="0" src="/content/ak15:504img5.gif" alt="${u(i)}$">
a usual random data generator did not fit. As the sequence
itself had been imposed certain
restrictions, the method of choosing the next random element
(in the interval defined by
restrictions) did not give the random sequence as a whole.
</p>
<p>
<br>
We have come to a conclusion that the problem can be solved in the following
way. If we arrange
all possible sequences in certain order (for example, in lexicographical
order) and assign each
sequence its number, after choice of the random number it is possible to
take the correspondent
sequence for the random one. At the first glance it seems enough to
make up a program generating
all these sequences in such order. Alas! Even having not great values
of <i>M</i> and <i>N</i> it would have
taken any powerful modern computer centuries to enumerate all such
sequences. It turned out it was
possible to avoid generating all sequences if we managed to create
required sequence according to
its number immediately. But even this statement does not cover all.
As the amount of sequences is
quite large, the number can be a long one, composed of hundreds decimal
digits, though our
random data generator could give only normal numbers. We decided to
produce a long random
number from a real random number distributed in [0,1]. Namely, present
the number in binary
notation: 
<img width="101" height="34" align="MIDDLE" border="0" src="/content/ak15:504img6.gif" alt="$0.b(1)b(2)dots$">,
where all <i>b</i>(<i>i</i>) = 0 or 1. Let us set a
regulation to associate such real number
to an integer from [<i>A</i>,<i>B</i>] segment:
</p><p>
</p><h3>Formula</h3>
<br><p></p>
<div align="CENTER">
<img width="666" height="76" src="/content/ak15:504img7.gif" alt="begin{displaymath}G(A,B,0.b_1b_2dots b_p) = left{ begin{array}{ll}
A, &amp; m...
...p, &amp; mbox{if $b_1=1$} end{array} right.
end{array} right.
end{displaymath}">
</div>
<br clear="ALL">
<p></p>

<p>
Here we suppose, that <img width="55" height="32" align="MIDDLE" border="0" src="/content/ak15:504img8.gif" alt="$A le B$">,
<img width="45" height="30" align="MIDDLE" border="0" src="/content/ak15:504img9.gif" alt="$p ge 0$">,
and ``div 2" is an integer
division by 2.
</p>
<p>
<br>

Let <i>M</i>, <i>N</i> (
<img width="144" height="32" align="MIDDLE" border="0" src="/content/ak15:504img10.gif" alt="$1 le N le M le 200$">)
and a binary real number
<img width="133" height="34" align="MIDDLE" border="0" src="/content/ak15:504img11.gif" alt="$0.b(1)b(2)dots b(p)$">
(
<img width="95" height="30" align="MIDDLE" border="0" src="/content/ak15:504img12.gif" alt="$1 le p le 400$">)
be given.
Write a program to find out the corresponding 
<img width="155" height="34" align="MIDDLE" border="0" src="/content/ak15:504img1.gif" alt="$u(1), u(2), dots, u(N)$">
sequence, i.e. to find a sequence
with 
<img width="197" height="34" align="MIDDLE" border="0" src="/content/ak15:504img13.gif" alt="$G(1, T, 0.b(1)b(2)dots b(p))$">
number in lexicographical order of all
possible <img width="52" height="34" align="MIDDLE" border="0" src="/content/ak15:504img5.gif" alt="${u(i)}$">
for the given
<i>M</i> and <i>N</i> (<i>T</i> is the quantity of such sequences). Numeration begins with 1.
Keep in mind that in
lexicographical order <img width="47" height="34" align="MIDDLE" border="0" src="/content/ak15:504img14.gif" alt="${l(i)}$">
proceeds <img width="52" height="34" align="MIDDLE" border="0" src="/content/ak15:504img15.gif" alt="${h(i)}$">
if after omitting equal
beginnings, the first number of

<img width="47" height="34" align="MIDDLE" border="0" src="/content/ak15:504img14.gif" alt="${l(i)}$">
tail is smaller than the first number or <img width="52" height="34" align="MIDDLE" border="0" src="/content/ak15:504img15.gif" alt="${h(i)}$">
tail.
Following example illustrates the list of all possible
sequences for <i>M</i> = 4 and <i>N</i> = 3 in lexicographical order.
</p><p>
</p><h3>A note (it does not concern the solution of this task):</h3>
<p>The choice of random binary vector 
<img width="133" height="34" align="MIDDLE" border="0" src="/content/ak15:504img11.gif" alt="$0.b(1)b(2)dots b(p)$">
does not give an
absolute uniform random
data generator if we use the Formula. However, taking into account the
fact that [<i>A</i>,<i>B</i>] interval is big
we shall obtain a distribution applicable in most cases.
</p><p>
</p><h3>Example</h3>
<pre>1, 2, 3
1, 2, 4
1, 3, 3
1, 3, 4
1, 4, 4
2, 2, 3
2, 2, 4
2, 3, 3
2, 3, 4
2, 4, 4
3, 3, 3
3, 3, 4
3, 4, 4
4, 4, 4
</pre>

<p>
(here <i>T</i>=14)
</p><p>
</p><h3>Input</h3>
<p>The first line of the input is an integer K ¡Ü 10, followed by K datasets.
</p><p>The first line of each dataset contains <i>M</i> and <i>N</i>. The second line
contains binary real
number 
<img width="133" height="34" align="MIDDLE" border="0" src="/content/ak15:504img11.gif" alt="$0.b(1)b(2)dots b(p)$">
(without leading, trailing and other spaces).
</p><p>
</p><h3>Output</h3>
<p>For each dataset, write into the output data file the corresponding sequence
<img width="155" height="34" align="MIDDLE" border="0" src="/content/ak15:504img1.gif" alt="$u(1), u(2), dots, u(N)$">.
The
sequence numbers should be separated with spaces and end-of-line characters.
There should be up to 20 numbers in each line. If neccesary, the numbers will have leading blanks to occupy 3 characters.
</p><p>
</p><h3>Example</h3>

<pre><b>Input:</b>

1
4 3
0.01101101011110010001101010001011010

<b>Output:</b>

  2   2   4
</pre>