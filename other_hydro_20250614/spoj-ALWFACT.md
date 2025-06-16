<p>Chico told his students that now they would be referenced by  numerical codes of up to 12 digits in official communications (e-mails  and tasks). And then he gave to each one of his students a card  containing an unique number written on it. Quickly the students assumed  that this would be their code, but to the surprise of the students and  Levi's despair, Professor Chico explained that these were not their  code.</p>
<p>A student's code was the term of an ordered sequence <strong>S </strong>that was in the position (indexed from 1) specified by the number on  the card of each student. This sequence has a special feature: each  term, when decomposed into prime factors, can only have numbers  contained in a set of <strong>N</strong> elements written on the board  by the teacher. And to make life even harder for Levi, those numbers  would change every week in such a way that he will always have to  recalculate his code if he doesn't want to delay his tasks.</p>
<p>Your task is to make a program to help Levi, so that given the  prime numbers written on the board during the week by Professor Chico  and number on the card, tell his weekly code.</p>
<h3>Input</h3>
<p>The input consists of several test cases. The first line of a test case contains two integers <strong>N</strong> (1 ¡Ü <strong>N</strong> ¡Ü 10<sup>2</sup>) and <strong>M </strong>(1 ¡Ü <strong>M</strong> ¡Ü 10<sup>5</sup>)  representing respectively the number of numbers written by Professor  Chico and the number written on the card. The second line contains <strong>N </strong>prime numbers <strong>P</strong><sub><strong>i </strong></sub>(2 ¡Ü <strong>P</strong><sub><strong>i</strong></sub> &lt; 10<sup>6</sup>), where <strong>P</strong><sub><strong>i</strong></sub> (1 ¡Ü <strong>i</strong> ¡Ü <strong>N</strong>) is a number written in the board. The entry ends when <strong>N</strong>=<strong>M</strong>=0.</p>
<h3>Output</h3>
<p>The output consists of one line per test case containing the Levi's weekly code.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2 1
</p><p>2 3
</p><p>2 10
</p><p>2 3
</p><p>3 10
</p><p>2 3 5
</p><p>3 10
</p><p>3 7 13
</p><p>0 0</p>

<strong>Output:</strong>
<p>2
</p><p>24
</p><p>15
</p><p>81</p></pre>