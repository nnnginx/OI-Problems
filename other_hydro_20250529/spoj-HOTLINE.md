<p>
Every customer sometimes needs help with new and unusual products. Therefore,
hotline service is very important for every company. We need a&nbsp;single phone
number where the customer can always find a&nbsp;friendly voice ready to help with
anything. On the other hand, many people are needed to serve as hotline
operators, and human resources are always very expensive. Moreover, it is not
easy to pretend "friendly voice" at 4am and explain to a&nbsp;drunken man that you
are really unable to give him the number to House of Parliament. It was
also found that some of the questions repeat very often and it is very
annoying to answer them again and again.

</p><p>
ACM is a&nbsp;modern company, wanting to solve its hotline problem. They want
to decrease the number of human operators by creating a&nbsp;complex software
system that would be able to answer most common questions. The customer's
voice is analysed by a&nbsp;special Voice Recognition Module (VRM) and converted
to a&nbsp;plain text. The text is then taken by an Artificial Automatic Adaptive
Answering Algorithm (AAAAA). The most common questions are recognised and
answered automatically. The replies are then converted to a&nbsp;sound by
Text-to-Speech Module (TTS).

</p><p>
You are to write the AAAAA module. Because your algorithm should be adaptive,
it has no explicit knowledge base. But it must be able to listen to sentences
in English and remember the mentioned facts. Whenever the question is asked
about such a&nbsp;fact, the system has to answer it properly. The VRM and TTS
modules are already implemented, so the input and output of AAAAA will be in
the text form.

</p><p>
</p><h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input. It stands
for the number of dialogues to follow. Each dialogue consists of zero or more
lines, each of them containing one sentence: either statement or question. The
statement ends with a&nbsp;dot character (<tt>.</tt>), the question ends with
a&nbsp;question mark (<tt>?</tt>). No statement will appear more than once, however
the questions can be repeated. There is one extra line after each dialogue.
That line ends with an&nbsp;exclamation mark (<tt>!</tt>).

</p><p>
Sentences can contain words, spaces and punctuation characters (such as
commas, colons, semicolons etc.). All words contain only letters of English
alphabet and are case-sensitive. That means the same word is always written
the same way, usually in lowercase. Acronyms, names and some other words can
begin with capital letters. For simplicity, all sentences begin with
a&nbsp;lowercase letter. Only if the first word should be written with a&nbsp;capital,
the sentence begins with a&nbsp;capital letter. There are no unneeded spaces
between words. No line will have more than 100 characters. There will be at
most 100 statements per each test case.

</p><p>

</p><h6 align="left">Statements</h6>

<p>
Each statement has one of the following two forms ( _ denotes a&nbsp;space):
<br>
<i>subject</i>  _<i>predicate</i>[<tt>s</tt>] [ _<i>object</i>] <tt>.</tt>
<br>
<i>subject</i>  _<tt>don't</tt>|<tt>doesn't</tt>  _<i>predicate</i> [ _<i>object</i>] <tt>.</tt>

</p><p>
The square brackets mark an&nbsp;optional part, the vertical line two possible
variants. Subject is a&nbsp;single word, noun or pronoun in singular. Predicate is
a&nbsp;verb (single word) denoting some activity. Object can be any text. Object
does not contain any dots. Any pair "verb + object" determines unique
activity. The same verb with different objects makes different independent
activities, i.e. the different and independent meaning of the sentence.
Sentence without any object can be considered as sentence with an&nbsp;empty
object. The verb without an&nbsp;object has different and independent meaning than
the same verb with any non-empty object.

</p><p>
The first variant of sentence denotes a&nbsp;positive statement. The word
"<i>predicate</i>[<tt>s</tt>]" means verb that matches the subject of the sentence.
If the subject is "<tt>I</tt>" or "<tt>you</tt>", the verb has the same form as the
infinitive. With any other subject, the letter "<tt>s</tt>" is appended on the
end of the verb. Assume there are no irregular verbs.

</p><p>
The second variant is a&nbsp;negative statement. Verb "<tt>don't</tt>" or
"<tt>doesn't</tt>" must also match the subject. The form "<tt>don't</tt>" is used
with either "<tt>I</tt>" or "<tt>you</tt>", "<tt>doesn't</tt>" is used in any other
case.

</p><p>
A&nbsp;special generic subject "<tt>everybody</tt>" can be used. It means the activity
holds for any subject. Other special subject is "<tt>nobody</tt>". Such sentence
also holds for any subject, but its meaning is negative. Both of these generic
subjects can be used with the first variant only (without "<tt>doesn't</tt>").
The sentence "<tt>nobody likes something</tt>" is exactly equal to
"<tt>everybody doesn't like something</tt>", except the latter form will never
occur in the input.

</p><p>

</p><h6 align="left">Questions</h6>

<p>
Each question has one of the following three forms:
</p><div align="left">
<dl compact="">
<dt>1.
</dt><dd><tt>do</tt>|<tt>does</tt>  _<i>subject</i>  _<i>predicate</i> [ _object] <tt>?</tt>
</dd><dt>2.
</dt><dd><tt>who</tt>  _<i>predicate</i><tt>s</tt> [ _<i>object</i>] <tt>?</tt>
</dd><dt>3.
</dt><dd><tt>what</tt>  _<tt>do</tt>|<tt>does</tt>  _<i>subject</i> <tt>do</tt> <tt>?</tt>
</dd></dl>
</div>
<p>
The word "<tt>do</tt>|<tt>does</tt>" always matches the subject ("<tt>do I?</tt>",
"<tt>do you?</tt>", "<tt>does</tt> any other subject?"). In the second
type of question, predicate always matches the word "<tt>who</tt>", i.e. the
"<tt>s</tt>" is always appended. Generic subjects cannot be used in questions.

</p><p>
</p><h3>Output</h3>

<p>
For each dialogue, your program must output the line <tt>Dialogue #</tt><var>D</var><tt>:</tt>,
where <var>D</var> is the sequence number of dialogue, starting with 1. Then print
exactly three lines for every question: the first line repeats the question,
the second line contains the answer, and the third line is empty. Print
nothing for statements. After each dialogue, print the same line with
an&nbsp;exclamation mark that was in the input. Then print one extra empty line.
Empty line contains a&nbsp;new-line character only.

</p><p>
The answer must be properly formated to be accepted by a&nbsp;TTS module. Only the
statements appearing in the input before the answer are used for the
corresponding reply. If there is any contradiction among statements, the
reply is always <tt>I am abroad.</tt>. If the question and statements consider
the special subject "<tt>you</tt>", it must be replaced with "<tt>I</tt>" in the
answer. If the question considers special subject "<tt>I</tt>", it must be
replaced with "<tt>you</tt>" in the answer. The verb must always match the
subject of the sentence. The exact form of the correct answer depends on the
type of question.

</p><p>

</p><h6 align="left">1.&nbsp;does subject predicate [object] ?</h6>

<p>
If there is any positive statement about the mentioned subject (or
generic subject "<tt>everybody</tt>"), predicate and object, the answer is:
<br>
<tt>yes,</tt>  _<i>subject</i>  _<i>predicate</i>[<tt>s</tt>] [ _<i>object</i>] <tt>.</tt>

</p><p>
If there is any negative statement about the mentioned subject (or
generic subject "<tt>nobody</tt>"), predicate and object, the answer is:
<br>
<tt>no,</tt>  _<i>subject</i>  _<tt>don't</tt>|<tt>doesn't</tt>  _<i>predicate</i> [ _<i>object</i>] <tt>.</tt>

</p><p>
Otherwise, the answer is:
<tt>maybe.</tt>

</p><p>
Subject in the answer is always the same subject as the subject of the
question.

</p><p>

</p><h6 align="left">2.&nbsp;who predicates [object] ?</h6>

<p>
If there is a&nbsp;positive statement considering any subject, the specified
predicate and object, the answer is:
<br>
<i>subject</i>  _<i>predicate</i>[<tt>s</tt>] [ _<i>object</i>] <tt>.</tt>

</p><p>
If two or more subjects match the activity, replace the subject in the answer
with enumeration of all such subjects, in the same order as the corresponding
statements have appeared in the input. Subjects are separated with comma and
space, last two subjects are separated with the word "<tt>and</tt>".
If "<tt>everybody</tt>" belongs to the group of enumerated subjects, do not
enumerate subjects, and print "<tt>everybody</tt>" only. If the enumeration
contains at least two subjects, the predicate matches the plural subject
(i.e. verb is without trailing "<tt>s</tt>"), otherwise it matches the only
subject.
<br>
<i>subject1</i> <tt>,</tt>  _<i>subject2</i>  _<tt>and</tt>  _<i>subject3</i> <i>predicate</i> [ _<i>object</i>] <tt>.</tt>

</p><p>
If there is a&nbsp;negative statement considering the generic subject "nobody",
the specified predicate and object, the answer is:
<br>
<i>nobody</i>  _<i>predicate</i><tt>s</tt> [ _<i>object</i>] <tt>.</tt>

</p><p>
Otherwise, the answer is:
<tt>I don't know.</tt>

</p><p>

</p><h6 align="left">3.&nbsp;what does subject do ?</h6>

<p>
If there are one or more sentences (both positive and negative) considering
the specified subject (or a&nbsp;generic subject "<tt>everybody</tt>" or "<tt>nobody</tt>"), all
verbs and objects from such sentences must be included in a&nbsp;reply in the same
order as the corresponding sentences have appeared in the input. No
verb-object pair can be included more than once (the eventual second
appearance must be skipped). The verb-object pairs are separated by a&nbsp;comma
followed by a&nbsp;space, the last verb is separated by a&nbsp;comma and the word
"<tt>and</tt>". Please note the comma is printed here although there was no comma
when separating the subjects in the previous type of answer (see above). The
negative answers have the same form as the statements, that means the verb
"<tt>don't</tt>" or "<tt>doesn't</tt>" is used:
<br>
<i>subject</i> [ _<tt>don't</tt>|<tt>doesn't</tt>]  _<i>predicate1</i>[<tt>s</tt>] [ _<i>object1</i>] <tt>,</tt>
<br>
[ _<tt>don't</tt>|<tt>doesn't</tt>]  _<i>predicate2</i>[<tt>s</tt>] [ _<i>object2</i>] <tt>,</tt>
<br>
_<tt>and</tt> [ _<tt>don't</tt>|<tt>doesn't</tt>]  _<i>predicate3</i>[<tt>s</tt>] [ _<i>object3</i>] <tt>.</tt>
<br>
<i>subject</i> [ _<tt>don't</tt>|<tt>doesn't</tt>]  _<i>predicate1</i>[<tt>s</tt>] [ _<i>object1</i>] <tt>,</tt>
<br>
_<tt>and</tt> [ _<tt>don't</tt>|<tt>doesn't</tt>]  _<i>predicate2</i>[<tt>s</tt>] [ _<i>object2</i>] <tt>.</tt>
<br>
<i>subject</i> [ _<tt>don't</tt>|<tt>doesn't</tt>]  _<i>predicate</i>[<tt>s</tt>] [ _<i>object</i>] <tt>.</tt>

</p><p>
Otherwise, the answer is:
<tt>I don't know.</tt>

</p><h3>Example</h3>
<p>Sample Input:</p>

<pre><tt>1
I like hotdogs.
nobody likes to work.
everybody smiles.
what do I do?
who smiles?
what do you do?
does Joe smile?
do I like to work?
everybody hurts sometimes.
who walks there?
Michal walks there.
who walks there?
what does Michal do?
do you understand?
nobody walks there.
do you understand now?
bye!
</tt></pre>

<p>Sample Output:</p>

<pre><tt>Dialogue #1:
what do I do?
you like hotdogs, don't like to work, and smile.

who smiles?
everybody smiles.

what do you do?
I don't like to work, and smile.

does Joe smile?
yes, Joe smiles.

do I like to work?
no, you don't like to work.

who walks there?
I don't know.

who walks there?
Michal walks there.

what does Michal do?
Michal doesn't like to work, smiles, hurts sometimes, and walks there.

do you understand?
maybe.

do you understand now?
I am abroad.

bye!
</tt></pre>