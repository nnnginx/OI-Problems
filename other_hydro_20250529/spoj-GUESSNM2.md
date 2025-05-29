<p>John has never been very good at maths. Due to his bad grades, his parents have sent him to the Academic Coalition of Mathematics (ACM). Despite the large amount of money his parents are spending on the ACM, John does not pay much attention during classes. However, today he has begun to think about all the effort his parents are putting into his education, and he has started to feel somewhat¡­  guilty. So he has made a decision: he is going to improve his maths grades!</p>
<div class="center"><img src="../../../content/elhipercubo:arithmetic.jpg" alt="" width="150" height="150"></div>
<p>However, no sooner had he resolved to pay attention than the lesson ended. So the only thing he has been able to do is to hurriedly copy the content of the blackboard in his notebook. Today, the teacher was explaining basic arithmetic expressions with unknowns. He vaguely remembers that his classmates have been substituting values into the unknowns to obtain the expressions¡¯ results. However, in all the hurry, John has only written down expressions, values and results in a messy fashion. So he does not know which value comes with each unknown, or which result goes with each expression.</p>
<p>That is the reason he needs your help: he wants to know, given an expression, some values and a result, whether it is possible or not to assign those values to the unknowns in order for the expression to evaluate to the given result. The particular assignment of values does not matter to John, as he wants to do it by himself. He only wants to know whether it is possible or not.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each test case in the input file consists of two lines:</p>
<ul class="itemize">
<li class="li-itemize"> The first line contains a sequence of natural numbers. The first one (1 ¡Ü <em>n</em> ¡Ü 5) is the number of unknowns that will occur in the expression. It is followed by a sequence of <em>n</em> integers <em>v</em><sub>1</sub> ¡­ <em>v</em><sub><em>n</em></sub> (0 ¡Ü <em>v</em><sub><em>i</em></sub> ¡Ü 50), which are the values to be assigned to the unknowns. Finally, there is an integer <em>m</em> (0 ¡Ü <em>m</em> ¡Ü 1000) representing the desired result of the evaluation of the expression. </li>
<li class="li-itemize">The second line contains an arithmetic expression composed of lowercase letters (<tt>a-z</tt>), brackets (<tt>(</tt> and <tt>)</tt>) and binary operators (<tt>+</tt>, <tt>-</tt>, <tt>*</tt>). This expression will contain <em>n</em> unknowns, represented by <em>n</em> different lowercase letters, without repetitions. The expression will not contain any blanks and will always be syntactically correct, i.e. it is just an unknown or has the form <tt>(</tt><em>e</em><sub>1</sub> <em>op</em> <em>e</em><sub>2</sub> <tt>)</tt>, where <em>e</em><sub>1</sub> and <em>e</em><sub>2</sub> are expressions and <em>op</em> is one of the three possible binary operators. </li>
</ul>
<p>The input will finish with a dummy test case of just one line containing <tt>0 0</tt>, which must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, print a single line with <tt>YES</tt> if there exists an assignment of the values <em>v</em><sub>1</sub> ¡­<em>v</em><sub><em>n</em></sub> to the unknowns such that the expression evaluates to <em>m</em>, and <tt>NO</tt> otherwise. Notice that each value <em>v</em><sub><em>i</em></sub> must be assigned to exactly one unknown.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<pre class="verbatim">3 2 3 4 14
((a+b)*c)
2 4 3 11
(a-b)
1 2 2
a
0 0
</pre>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<pre class="verbatim">YES
NO
YES
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemstter: Enrique Mart¨ªn Mart¨ªn</em></blockquote>