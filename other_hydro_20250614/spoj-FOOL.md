<p>
Surely you know someone who thinks he is very clever. You decide to
let him
down with the following problem:<br>
</p>
<ul>
  <li>"Can you tell me what the syntax for a set is?", you ask him.</li>
  <li>"Sure!", he replies, "a set encloses a
possibly empty list
of elements within two curly braces. Each element is either another set
or a letter of
the given alphabet. Elements in a list are separated by a comma." </li>
  <li>"So if I give you a word, can you tell me if it is a
syntactically
correct
representation of a set?" </li>
  <li>"Of course, any fool can do it!" is his answer.</li>
</ul>
<p>
Now you got him! You present him with the following grammar, defining
formally the syntax for a set (which was described informally by him):</p>
<pre>Set          ::= "{" Elementlist "}"
Elementlist  ::= &lt;empty&gt; | List
List         ::= Element | Element "," List
Element      ::= Atom | Set
Atom         ::= "{" | "}" | ","
</pre>
<p>
&lt;empty&gt; stands for the empty word, i.e. the list in a set can be empty.<br>
Soon he realizes that this task is much harder than he has thought,
since the alphabet consists of the characters
which are also used for the syntax of the set. So he claims that it is
not possible to decide efficiently if a word
consisting of <samp>"{"</samp>, <samp>"}"</samp> and <samp>","</samp> is a syntactically correct
representation of a set or not.<br>
To disprove him, you need to write an efficient program that will
decide this
problem.</p>
<h3>Input Specification</h3>
<p>The first line of the input file contains a number representing the
number of lines to follow. <br>
Each line consists of a word, for which your
program has to decide
if it is a syntactically correct representation of a set.
You may assume that each word consists of between <i>1</i> and <i>200</i>
characters
from the set { <samp>"{", "}", ","</samp> }.
</p>
<h3>Output Specification</h3>
<p>Output for each test case whether the word is a set or not.
Adhere to the format shown in the sample output.
</p>
<h3>Sample Input</h3>
<pre>4
{}
{{}}
{{}},{,}}
{,,}
</pre>
<h3>Sample Output</h3>
<pre>Word #1: Set
Word #2: Set
Word #3: Set
Word #4: No Set
</pre>