<p>Every student needs help from getting new knowledge by asking questions. Surveys are suggesting that some similar questions are repeated frequently. So it will be nice to develop an automatic question-answering system to answer these questions. Your algorithm should not have any prior knowledge, but it must be able to read sentences and remember the mentioned facts. Whenever the question is asked about such a fact, the system has to answer it properly.</p>
<h3>Input</h3>
<p>The input consists of many dialogues.</p>
<p>There is a single positive integer T on the first line of input, which denotes the number of following dialogues.(T &lt;= 500, but note that 95% of them are relatively small.) Each dialogue includes one or more lines. Each line contains one sentence: either a statement or a question. Statements end with a dot character (.) while questions end with a question mark (?). There is one extra line after each dialogue. That line ends with an exclamation mark (!). The definitions of the statements and questions will be discussed later.</p>
<p>Sentences can contain words, spaces and punctuation characters. All words contain only Latin letters and are case-sensitive. <strong>Unlike the normal English writing rules, the first letter of a sentence should keep lowercase unless the first word itself should begin with a capital letter.</strong> There are no extra spaces between words. No word will have more than 10 characters. There will be at most 1000 lines per dialogue.</p>
<p><strong>Statements</strong></p>
<p>Each statement has one of the following forms:</p>
<pre><em>
noun_phrase are noun_phrase.
noun_phrase can verb_phrase.
everything which can verb_phrase can verb_phrase.
everything which can verb_phrase are noun_phrase.
</em></pre>
<p><strong>noun_phrase and verb_phrase are both single word.</strong> The meanings of the four forms are:</p>
<pre>A are B: If X is A, then X is B.
A can B: If X is A, then X has the ability to B.
everything which can A can B: If X has the ability to A, X has the ability to B.
everything which can A are B: If X has the ability to A, X is B.
</pre>
<p><strong>Questions</strong></p>
<p>Each question has one of the following forms:</p>
<pre><em>
are noun_phrase noun_phrase?
can noun_phrase verb_phrase?
can everything which can verb_phrase verb_phrase?
are everything which can verb_phrase noun_phrase?
</em></pre>
<p>They are the question forms of the statements.</p>
<p>In each test case, the number of different noun phrases will not exceed 100; the number of different verb phrases will not exceed 100.</p>
<h3>Output</h3>
<p>For each test case, output two lines. The first line describes the test case number counting from 1, while the second line contains the same number of characters as the number of questions in this test case. Each character is either <strong>Y</strong>(denoting you can get that fact logically) or <strong>M</strong>(otherwise), without quotes. See the example.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
flies can fly.
flies are insects.
everything which can fly are animals.
are everything which can fly insects?
are flies animals?
can flies eat?
everything which can fly can eat.
can flies eat?
Bye!

<strong>Output:</strong>
Case #1:
MYMY
</pre>
<p><em>This problem is first solved by team </em><strong>Seraphim</strong> (Shanghai Jiao Tong University) <em>at 66 minutes after the onsite contest starts.</em></p>