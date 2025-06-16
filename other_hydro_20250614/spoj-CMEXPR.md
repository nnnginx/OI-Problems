<p>
The most important activity of ACM is the GSM network. As the mobile phone
operator, ACM must build its own transmitting stations. It is very important
to compute the exact behaviour of electro-magnetic waves. Unfortunately,
prediction of electro-magnetic fields is a&nbsp;very complex task and the
formulas describing them are very long and hard-to-read. For
example, Maxwell's Equations describing the basic laws of
electrical engineering are really tough.
</p><p>
ACM has designed its own computer system that can make some field
computations and produce results in the form of mathematic expressions.
Unfortunately, by generating the expression in several steps, there are
always some unneeded parentheses inside the expression. Your task is to take
these partial results and make them "nice" by removing all unnecessary
parentheses.
</p>
<h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 10000). It stands
for the number of expressions to follow. Each expression consists of a&nbsp;single
line containing only lowercase letters, operators (<tt>+</tt>, <tt>-</tt>, <tt>*</tt>,
<tt>/</tt>) and parentheses (<tt>(</tt> and <tt>)</tt>). The letters are variables
that can have any value, operators and parentheses have their usual meaning.
Multiplication and division have higher priority then subtraction and
addition. All operations with the same priority are computed from left to
right (operators are left-associative). There are no spaces inside the
expressions. No input line contains more than 250 characters.

</p><p>
</p><h3>Output</h3>

<p>
Print a&nbsp;single line for every expression. The line must contain the same
expression with unneeded parentheses removed. You must remove as many
parentheses as possible without changing the semantics of the expression.
The semantics of the expression is considered the same if and only if any of
the following conditions hold:
</p><div align="left">
<ul>
<li>The ordering of operations remains the same. That means "(<var>a</var>+<var>b</var>)+<var>c</var>" is
  the same as "<var>a</var>+<var>b</var>+<var>c</var>", and "<var>a</var>+(<var>b</var>/<var>c</var>)" is the same as "<var>a</var>+<var>b</var>/<var>c</var>".
</li><li>The order of some operations is swapped but the result remains unchanged
  with respect to the addition and multiplication associativity.
  That means "<var>a</var>+(<var>b</var>+<var>c</var>)" and "(<var>a</var>+<var>b</var>)+<var>c</var>" are the same. We can also combine
  addition with subtraction and multiplication with division, if the
  subtraction or division is the second operation. For example, "<var>a</var>+(<var>b</var>-<var>c</var>)"
  is the same as "<var>a</var>+<var>b</var>-<var>c</var>".
</li></ul>
</div>
<p>
You cannot use any other laws, namely you cannot swap left and right
operands and you cannot replace "<var>a</var>-(<var>b</var>-<var>c</var>)" with "<var>a</var>-<var>b</var>+<var>c</var>".

</p><h3>Example</h3>
<p>Sample Input:</p>

<pre><tt>8
(a+(b*c))
((a+b)*c)
(a*(b*c))
(a*(b/c)*d)
((a/(b/c))/d)
((x))
(a+b)-(c-d)-(e/f)
(a+b)+(c-d)-(e+f)
</tt></pre>

<p>Sample Output:</p>

<pre><tt>a+b*c
(a+b)*c
a*b*c
a*b/c*d
a/(b/c)/d
x
a+b-(c-d)-e/f
a+b+c-d-(e+f)
</tt></pre>